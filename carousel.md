# Carousel Component Examples

## Example 1: Basic Carousel with Arrows

```html
<div class="relative">
    <!-- Carousel container -->
    <div class="overflow-hidden relative">
        <!-- Carousel wrapper -->
        <div class="flex transition-transform duration-500 ease-in-out" style="transform: translateX(0%);">
            <!-- Slide 1 -->
            <div class="w-full flex-shrink-0">
                <img src="https://images.unsplash.com/photo-1518791841217-8f162f1e1131?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80" class="w-full h-64 object-cover rounded-lg" alt="Slide 1">
            </div>
        </div>
    </div>
    
    <!-- Previous Button -->
    <button type="button" class="absolute top-1/2 left-4 -translate-y-1/2 bg-white/80 hover:bg-white text-gray-800 p-2 rounded-full shadow">
        <i class="ri-arrow-left-s-line text-xl"></i>
    </button>
    
    <!-- Next Button -->
    <button type="button" class="absolute top-1/2 right-4 -translate-y-1/2 bg-white/80 hover:bg-white text-gray-800 p-2 rounded-full shadow">
        <i class="ri-arrow-right-s-line text-xl"></i>
    </button>
</div>
```

## Example 2: Carousel with Indicators

```html
<div class="relative">
    <!-- Carousel container -->
    <div class="overflow-hidden relative h-64 rounded-lg">
        <!-- Slides (stacked) -->
        <div class="absolute inset-0 fade-in">
            <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80" class="w-full h-full object-cover" alt="Mountain">
        </div>
        
        <!-- Overlay for text -->
        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent"></div>
        
        <!-- Caption -->
        <div class="absolute bottom-0 left-0 right-0 p-4 text-white">
            <h3 class="font-bold text-lg">Beautiful Mountains</h3>
            <p class="text-sm">Explore the majestic landscapes and breathtaking views.</p>
        </div>
    </div>
    
    <!-- Indicators -->
    <div class="flex justify-center mt-4">
        <button type="button" class="w-3 h-3 mx-1 rounded-full bg-blue-500"></button>
        <button type="button" class="w-3 h-3 mx-1 rounded-full bg-gray-300 hover:bg-gray-400"></button>
        <button type="button" class="w-3 h-3 mx-1 rounded-full bg-gray-300 hover:bg-gray-400"></button>
        <button type="button" class="w-3 h-3 mx-1 rounded-full bg-gray-300 hover:bg-gray-400"></button>
    </div>
</div>
```

## Example 3: Carousel with Thumbnails

```html
<div>
    <!-- Main image -->
    <div class="overflow-hidden rounded-lg mb-4">
        <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80" class="w-full h-64 object-cover" alt="Main Image">
    </div>
    
    <!-- Thumbnails -->
    <div class="flex space-x-2 overflow-x-auto pb-2">
        <button class="flex-shrink-0 border-2 border-blue-500 rounded-md overflow-hidden">
            <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=200&q=80" class="h-16 w-24 object-cover" alt="Thumbnail 1">
        </button>
        <button class="flex-shrink-0 border-2 border-transparent hover:border-gray-300 rounded-md overflow-hidden">
            <img src="https://images.unsplash.com/photo-1433838552652-f9a46b332c40?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=200&q=80" class="h-16 w-24 object-cover" alt="Thumbnail 2">
        </button>
        <button class="flex-shrink-0 border-2 border-transparent hover:border-gray-300 rounded-md overflow-hidden">
            <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=200&q=80" class="h-16 w-24 object-cover" alt="Thumbnail 3">
        </button>
        <button class="flex-shrink-0 border-2 border-transparent hover:border-gray-300 rounded-md overflow-hidden">
            <img src="https://images.unsplash.com/photo-1518098268026-4e89f1a2cd8e?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=200&q=80" class="h-16 w-24 object-cover" alt="Thumbnail 4">
        </button>
    </div>
</div>
```

## Example 4: Product Carousel

```html
<div class="relative">
    <!-- Carousel header with title and navigation -->
    <div class="flex items-center justify-between mb-4">
        <h3 class="text-lg font-medium text-gray-800">Featured Products</h3>
        <div class="flex space-x-2">
            <button type="button" class="p-1 rounded-full border border-gray-300 hover:bg-gray-100">
                <i class="ri-arrow-left-s-line text-lg"></i>
            </button>
            <button type="button" class="p-1 rounded-full border border-gray-300 hover:bg-gray-100">
                <i class="ri-arrow-right-s-line text-lg"></i>
            </button>
        </div>
    </div>
    
    <!-- Product carousel -->
    <div class="overflow-x-auto carousel-snap">
        <div class="flex -mx-2 pb-2">
            <!-- Product 1 -->
            <div class="w-1/2 md:w-1/3 lg:w-1/4 px-2 flex-shrink-0">
                <div class="bg-white rounded-lg border border-gray-200 overflow-hidden">
                    <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=300&q=80" alt="Product" class="w-full h-40 object-cover">
                    <div class="p-4">
                        <h4 class="text-sm font-medium text-gray-900">Premium Watch</h4>
                        <p class="text-sm text-gray-500 mb-2">Elegant design</p>
                        <div class="flex items-center justify-between">
                            <span class="font-bold text-gray-900">$99.99</span>
                            <button class="bg-blue-500 text-white text-xs rounded-full p-1">
                                <i class="ri-shopping-cart-line"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Additional Products -->
            <!-- Product 2, 3, 4, etc. would follow the same pattern -->
        </div>
    </div>
</div>
```

## Example 5: Hero Carousel

```html
<div class="relative">
    <!-- Hero carousel with full-width slides -->
    <div class="overflow-hidden rounded-lg relative h-80">
        <!-- Current slide -->
        <div class="absolute inset-0">
            <div class="absolute inset-0 bg-black/40"></div>
            <img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80" class="w-full h-full object-cover" alt="Restaurant">
            
            <!-- Content -->
            <div class="absolute inset-0 flex flex-col items-center justify-center p-4 text-center text-white">
                <h3 class="text-2xl md:text-4xl font-bold mb-2">Delicious Cuisine</h3>
                <p class="text-base md:text-xl mb-4">Discover our chef's special dishes</p>
                <button class="bg-white text-gray-800 hover:bg-gray-100 font-medium py-2 px-4 rounded-lg transition-colors duration-200">
                    Book a Table
                </button>
            </div>
        </div>
    </div>
    
    <!-- Navigation arrows -->
    <button type="button" class="absolute top-1/2 left-4 -translate-y-1/2 bg-white/30 hover:bg-white/50 text-white p-2 rounded-full backdrop-blur-sm">
        <i class="ri-arrow-left-s-line text-xl"></i>
    </button>
    <button type="button" class="absolute top-1/2 right-4 -translate-y-1/2 bg-white/30 hover:bg-white/50 text-white p-2 rounded-full backdrop-blur-sm">
        <i class="ri-arrow-right-s-line text-xl"></i>
    </button>
    
    <!-- Progress bar -->
    <div class="absolute bottom-4 left-0 right-0 flex justify-center space-x-2">
        <div class="h-1 w-16 bg-white rounded-full"></div>
        <div class="h-1 w-16 bg-white/30 rounded-full"></div>
        <div class="h-1 w-16 bg-white/30 rounded-full"></div>
    </div>
</div>
```
