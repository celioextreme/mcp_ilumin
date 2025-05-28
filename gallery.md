# Gallery Component Examples

## Example 1: Basic Image Gallery Grid
```html
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
    <div class="aspect-square overflow-hidden rounded-lg">
        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb" 
             alt="Landscape" 
             class="w-full h-full object-cover hover:scale-110 transition-transform duration-500">
    </div>
    <div class="aspect-square overflow-hidden rounded-lg">
        <img src="https://images.unsplash.com/photo-1454496522488-7a8e488e8606" 
             alt="Mountains" 
             class="w-full h-full object-cover hover:scale-110 transition-transform duration-500">
    </div>
    <!-- More gallery items -->
</div>
```

## Example 2: Gallery with Overlay Effects
```html
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
    <div class="gallery-item relative rounded-lg overflow-hidden group cursor-pointer">
        <img src="https://images.unsplash.com/photo-1477959858617-67f85cf4f1df" 
             alt="City Skyline" 
             class="w-full h-64 object-cover">
        <div class="gallery-overlay absolute inset-0 bg-black bg-opacity-60 opacity-0 flex flex-col items-center justify-center p-4">
            <h3 class="text-white font-medium text-lg mb-2">Urban Landscape</h3>
            <p class="text-gray-200 text-sm text-center">Modern city skyline at sunset</p>
            <button class="mt-4 px-4 py-2 bg-white text-gray-900 rounded-md hover:bg-gray-100 transition">
                <i class="ri-eye-line mr-2"></i> View
            </button>
        </div>
    </div>
    <!-- More gallery items with overlay -->
</div>

<style>
    .gallery-overlay {
        transition: opacity 0.3s ease;
    }
    
    .gallery-item:hover .gallery-overlay {
        opacity: 1;
    }
</style>
```

## Example 3: Masonry Gallery Layout
```html
<div class="masonry-grid">
    <div class="masonry-grid-item">
        <img src="https://images.unsplash.com/photo-1496449903678-68ddcb189a24" 
             alt="Tall Building" 
             class="w-full rounded-lg shadow-sm">
    </div>
    <div class="masonry-grid-item">
        <img src="https://images.unsplash.com/photo-1451337516015-6b6e9a44a8a3" 
             alt="Small Landscape" 
             class="w-full rounded-lg shadow-sm">
    </div>
    <!-- More masonry items -->
</div>

<style>
    .masonry-grid {
        column-count: 1;
    }
    
    @media (min-width: 640px) {
        .masonry-grid {
            column-count: 2;
        }
    }
    
    @media (min-width: 768px) {
        .masonry-grid {
            column-count: 3;
        }
    }
    
    .masonry-grid-item {
        break-inside: avoid;
        margin-bottom: 1rem;
    }
</style>
```

## Example 4: Filterable Gallery
```html
<div class="mb-6">
    <div class="flex flex-wrap gap-2">
        <button class="px-4 py-2 bg-indigo-600 text-white rounded-md filter-btn active" data-filter="all">
            All
        </button>
        <button class="px-4 py-2 bg-gray-200 text-gray-700 rounded-md hover:bg-gray-300 filter-btn" data-filter="nature">
            Nature
        </button>
        <button class="px-4 py-2 bg-gray-200 text-gray-700 rounded-md hover:bg-gray-300 filter-btn" data-filter="architecture">
            Architecture
        </button>
        <button class="px-4 py-2 bg-gray-200 text-gray-700 rounded-md hover:bg-gray-300 filter-btn" data-filter="travel">
            Travel
        </button>
    </div>
</div>
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 filter-gallery">
    <div class="gallery-item" data-category="nature">
        <img src="https://images.unsplash.com/photo-1472214103451-9374bd1c798e" 
             alt="Forest Valley" 
             class="w-full h-48 object-cover rounded-lg">
        <div class="mt-2">
            <h3 class="text-sm font-medium text-gray-700">Forest Valley</h3>
            <p class="text-xs text-gray-500">Nature</p>
        </div>
    </div>
    <!-- More filterable items -->
</div>

<script>
    // Filterable Gallery
    const filterBtns = document.querySelectorAll('.filter-btn');
    const galleryItems = document.querySelectorAll('.filter-gallery .gallery-item');
    
    filterBtns.forEach(btn => {
        btn.addEventListener('click', function() {
            // Remove active class from all buttons
            filterBtns.forEach(btn => {
                btn.classList.remove('bg-indigo-600', 'text-white');
                btn.classList.add('bg-gray-200', 'text-gray-700');
            });
            
            // Add active class to clicked button
            this.classList.remove('bg-gray-200', 'text-gray-700');
            this.classList.add('bg-indigo-600', 'text-white');
            
            const filter = this.getAttribute('data-filter');
            
            galleryItems.forEach(item => {
                if (filter === 'all' || item.getAttribute('data-category') === filter) {
                    item.style.display = 'block';
                } else {
                    item.style.display = 'none';
                }
            });
        });
    });
</script>
```

## Example 5: Lightbox Gallery
```html
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4 lightbox-gallery">
    <div class="lightbox-item cursor-pointer" data-img-src="https://images.unsplash.com/photo-1506744038136-46273834b3fb">
        <div class="aspect-w-1 aspect-h-1 overflow-hidden rounded-lg">
            <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?w=500" 
                 alt="Landscape" 
                 class="w-full h-full object-cover hover:opacity-90 transition-opacity duration-300">
            <div class="absolute inset-0 bg-black bg-opacity-20 opacity-0 hover:opacity-100 flex items-center justify-center transition-opacity">
                <i class="ri-zoom-in-line text-white text-2xl"></i>
            </div>
        </div>
        <p class="text-xs text-gray-500 mt-1">Landscape View</p>
    </div>
    <!-- More lightbox items -->
</div>

<!-- Lightbox Modal (Hidden by default) -->
<div id="lightboxModal" class="fixed inset-0 z-50 hidden">
    <div class="absolute inset-0 bg-black bg-opacity-90 gallery-lightbox"></div>
    <div class="absolute top-4 right-4">
        <button id="closeLightbox" class="text-white p-2 hover:text-gray-300 transition-colors">
            <i class="ri-close-line text-3xl"></i>
        </button>
    </div>
    <div class="absolute inset-x-0 bottom-4">
        <p id="lightboxCaption" class="text-center text-white text-sm"></p>
    </div>
    <div class="absolute inset-0 flex items-center justify-center p-4">
        <div class="relative max-w-4xl w-full">
            <button id="prevBtn" class="absolute left-0 top-1/2 transform -translate-y-1/2 -translate-x-12 text-white p-2 hover:text-gray-300 transition-colors">
                <i class="ri-arrow-left-line text-3xl"></i>
            </button>
            <img id="lightboxImage" src="" alt="Lightbox Image" class="max-h-[80vh] mx-auto">
            <button id="nextBtn" class="absolute right-0 top-1/2 transform -translate-y-1/2 translate-x-12 text-white p-2 hover:text-gray-300 transition-colors">
                <i class="ri-arrow-right-line text-3xl"></i>
            </button>
        </div>
    </div>
</div>

<script>
    // Lightbox Gallery
    const lightboxItems = document.querySelectorAll('.lightbox-item');
    const lightboxModal = document.getElementById('lightboxModal');
    const lightboxImage = document.getElementById('lightboxImage');
    const lightboxCaption = document.getElementById('lightboxCaption');
    const closeLightbox = document.getElementById('closeLightbox');
    const prevBtn = document.getElementById('prevBtn');
    const nextBtn = document.getElementById('nextBtn');
    let currentIndex = 0;
    
    // Show lightbox
    lightboxItems.forEach((item, index) => {
        item.addEventListener('click', function() {
            currentIndex = index;
            const imgSrc = item.getAttribute('data-img-src');
            const caption = item.querySelector('p').textContent;
            
            lightboxImage.src = imgSrc;
            lightboxCaption.textContent = caption;
            lightboxModal.classList.remove('hidden');
        });
    });
    
    // Close lightbox and navigation functions
    // ... (additional JavaScript for navigation)
</script>
```
