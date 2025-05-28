# Tailwind CSS Images Examples

## Example 1: Basic Image Styling

```html
<div class="space-y-8">
    <!-- Rounded corners -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Rounded Corners</h3>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
            <div>
                <p class="text-sm text-gray-600 mb-1">Slightly Rounded</p>
                <img src="https://images.unsplash.com/photo-1682687982107-14492010e05e" alt="Mountain landscape" class="rounded-md w-full h-40 object-cover">
            </div>
            <div>
                <p class="text-sm text-gray-600 mb-1">More Rounded</p>
                <img src="https://images.unsplash.com/photo-1682687982107-14492010e05e" alt="Mountain landscape" class="rounded-xl w-full h-40 object-cover">
            </div>
            <div>
                <p class="text-sm text-gray-600 mb-1">Fully Rounded</p>
                <img src="https://images.unsplash.com/photo-1682687982107-14492010e05e" alt="Mountain landscape" class="rounded-full w-full h-40 object-cover">
            </div>
        </div>
    </div>
    
    <!-- Object fit variations -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Object Fit Variations</h3>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
            <div>
                <p class="text-sm text-gray-600 mb-1">object-cover</p>
                <img src="https://images.unsplash.com/photo-1493246507139-91e8fad9978e" alt="Landscape" class="border-2 border-gray-300 w-full h-40 object-cover">
            </div>
            <div>
                <p class="text-sm text-gray-600 mb-1">object-contain</p>
                <img src="https://images.unsplash.com/photo-1493246507139-91e8fad9978e" alt="Landscape" class="border-2 border-gray-300 w-full h-40 object-contain">
            </div>
            <div>
                <p class="text-sm text-gray-600 mb-1">object-fill</p>
                <img src="https://images.unsplash.com/photo-1493246507139-91e8fad9978e" alt="Landscape" class="border-2 border-gray-300 w-full h-40 object-fill">
            </div>
        </div>
    </div>
</div>
```

## Example 2: Image with Overlay and Captions

```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <!-- Image with text overlay -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Text Overlay</h3>
        <div class="relative overflow-hidden rounded-lg group">
            <img 
                src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4" 
                alt="Mountain range" 
                class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110"
            >
            <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                <div class="p-4 text-white">
                    <h4 class="text-xl font-bold">Mountain Range</h4>
                    <p class="text-sm opacity-80">A beautiful view of the mountains</p>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Hover reveal caption -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Hover Reveal Caption</h3>
        <div class="relative overflow-hidden rounded-lg group">
            <img 
                src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e" 
                alt="Lake and mountains" 
                class="w-full h-64 object-cover"
            >
            <div class="absolute inset-0 bg-blue-800/75 flex items-center justify-center opacity-0 transition-opacity duration-300 group-hover:opacity-100">
                <div class="text-white text-center p-4 transform translate-y-4 transition-transform duration-300 group-hover:translate-y-0">
                    <h4 class="text-xl font-bold mb-2">Tranquil Lake</h4>
                    <p class="text-sm">Hover to see this caption overlay appear with a smooth transition</p>
                    <button class="mt-2 px-4 py-1 bg-white text-blue-800 text-sm rounded-full">View Details</button>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 3: Advanced Image Effects

```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    <!-- Grayscale effect -->
    <div>
        <h3 class="text-base font-medium text-gray-700 mb-2">Grayscale Effect</h3>
        <div class="relative overflow-hidden rounded-lg">
            <img 
                src="https://images.unsplash.com/photo-1444464666168-49d633b86797" 
                alt="Colorful birds" 
                class="w-full h-56 object-cover grayscale hover:grayscale-0 transition-all duration-500"
            >
        </div>
        <p class="text-sm text-gray-500 mt-2">Hover to see colors</p>
    </div>
    
    <!-- Blur effect -->
    <div>
        <h3 class="text-base font-medium text-gray-700 mb-2">Blur Effect</h3>
        <div class="relative overflow-hidden rounded-lg">
            <img 
                src="https://images.unsplash.com/photo-1516214104703-d870798883c5" 
                alt="Mountain landscape" 
                class="w-full h-56 object-cover blur-sm hover:blur-none transition-all duration-500"
            >
        </div>
        <p class="text-sm text-gray-500 mt-2">Hover to clear the blur</p>
    </div>
    
    <!-- Zoom effect -->
    <div>
        <h3 class="text-base font-medium text-gray-700 mb-2">Zoom Effect</h3>
        <div class="relative overflow-hidden rounded-lg">
            <img 
                src="https://images.unsplash.com/photo-1505765050516-f72dcac9c60e" 
                alt="Forest landscape" 
                class="w-full h-56 object-cover transform hover:scale-125 transition-transform duration-700"
            >
        </div>
        <p class="text-sm text-gray-500 mt-2">Hover to zoom in</p>
    </div>
</div>
```

## Example 4: Image Gallery and Grid Layouts

```html
<div class="space-y-6">
    <!-- Basic grid gallery -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Basic Grid Gallery</h3>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-2">
            <img src="https://images.unsplash.com/photo-1447752875215-b2761acb3c5d" alt="Nature" class="w-full h-32 object-cover rounded">
            <img src="https://images.unsplash.com/photo-1433086966358-54859d0ed716" alt="Waterfall" class="w-full h-32 object-cover rounded">
            <img src="https://images.unsplash.com/photo-1470252649378-9c29740c9fa8" alt="Sunset" class="w-full h-32 object-cover rounded">
            <img src="https://images.unsplash.com/photo-1505144808419-1957a94ca61e" alt="Mountains" class="w-full h-32 object-cover rounded">
        </div>
    </div>
    
    <!-- Masonry-style gallery -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Pinterest-Style Masonry Layout</h3>
        <div class="grid grid-cols-2 md:grid-cols-3 gap-3">
            <div class="space-y-3">
                <img src="https://images.unsplash.com/photo-1414609245224-afa02bfb3fda" alt="Nature" class="w-full rounded shadow-sm hover:shadow-md transition-shadow">
                <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef" alt="Mountain" class="w-full rounded h-40 object-cover shadow-sm hover:shadow-md transition-shadow">
            </div>
            <div class="space-y-3">
                <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470" alt="Landscape" class="w-full h-52 rounded object-cover shadow-sm hover:shadow-md transition-shadow">
                <img src="https://images.unsplash.com/photo-1439853949127-fa647821eba0" alt="Lake" class="w-full rounded shadow-sm hover:shadow-md transition-shadow">
            </div>
            <div class="space-y-3 hidden md:block">
                <img src="https://images.unsplash.com/photo-1455218873509-8097305ee378" alt="Forest" class="w-full h-44 rounded object-cover shadow-sm hover:shadow-md transition-shadow">
                <img src="https://images.unsplash.com/photo-1473773508845-188df298d2d1" alt="Mountains" class="w-full rounded h-48 object-cover shadow-sm hover:shadow-md transition-shadow">
            </div>
        </div>
    </div>
</div>
```

## Example 5: Practical Image Components

```html
<div class="space-y-8">
    <!-- User avatar with status -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-3">User Avatars with Status</h3>
        <div class="flex flex-wrap gap-6 items-end">
            <div class="flex flex-col items-center">
                <div class="relative">
                    <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="User Avatar" class="w-16 h-16 rounded-full">
                    <span class="absolute bottom-0 right-0 w-4 h-4 bg-green-500 border-2 border-white rounded-full"></span>
                </div>
                <span class="text-sm text-gray-600 mt-1">Online</span>
            </div>
            
            <div class="flex flex-col items-center">
                <div class="relative">
                    <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="User Avatar" class="w-16 h-16 rounded-full">
                    <span class="absolute bottom-0 right-0 w-4 h-4 bg-red-500 border-2 border-white rounded-full"></span>
                </div>
                <span class="text-sm text-gray-600 mt-1">Busy</span>
            </div>
            
            <div class="flex flex-col items-center">
                <div class="relative">
                    <img src="https://randomuser.me/api/portraits/men/86.jpg" alt="User Avatar" class="w-16 h-16 rounded-full">
                    <span class="absolute bottom-0 right-0 w-4 h-4 bg-gray-400 border-2 border-white rounded-full"></span>
                </div>
                <span class="text-sm text-gray-600 mt-1">Away</span>
            </div>
            
            <div class="flex flex-col items-center">
                <div class="relative">
                    <div class="w-16 h-16 rounded-full bg-gray-200 flex items-center justify-center text-gray-600 text-xl font-medium">
                        JD
                    </div>
                    <span class="absolute bottom-0 right-0 w-4 h-4 bg-yellow-500 border-2 border-white rounded-full"></span>
                </div>
                <span class="text-sm text-gray-600 mt-1">Idle</span>
            </div>
        </div>
    </div>
</div>
```
