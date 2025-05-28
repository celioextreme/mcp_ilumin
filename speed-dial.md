# Speed Dial Component Examples

## Example 1: Basic Speed Dial
```html
<div class="relative inline-block h-full w-full">
    <div class="absolute bottom-4 right-4">
        <div class="group">
            <!-- Main Button -->
            <button class="flex items-center justify-center w-14 h-14 rounded-full bg-blue-600 text-white shadow-lg hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500">
                <i class="ri-add-line text-2xl"></i>
            </button>
            
            <!-- Speed Dial Options -->
            <div class="absolute bottom-16 right-0 mb-2 hidden group-hover:block">
                <div class="flex flex-col-reverse items-center space-y-reverse space-y-2">
                    <!-- Option 1 -->
                    <div class="flex items-center">
                        <span class="bg-gray-800 text-white text-sm px-3 py-1 rounded-md mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-200">Edit</span>
                        <button class="flex items-center justify-center w-10 h-10 rounded-full bg-green-500 text-white shadow-lg hover:bg-green-600">
                            <i class="ri-edit-line"></i>
                        </button>
                    </div>
                    
                    <!-- Option 2 -->
                    <div class="flex items-center">
                        <span class="bg-gray-800 text-white text-sm px-3 py-1 rounded-md mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-200">Share</span>
                        <button class="flex items-center justify-center w-10 h-10 rounded-full bg-blue-500 text-white shadow-lg hover:bg-blue-600">
                            <i class="ri-share-line"></i>
                        </button>
                    </div>
                    
                    <!-- Option 3 -->
                    <div class="flex items-center">
                        <span class="bg-gray-800 text-white text-sm px-3 py-1 rounded-md mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-200">Delete</span>
                        <button class="flex items-center justify-center w-10 h-10 rounded-full bg-red-500 text-white shadow-lg hover:bg-red-600">
                            <i class="ri-delete-bin-line"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 2: Animated Speed Dial with Direction Options
```html
<!-- Vertical Direction -->
<div class="relative h-full">
    <div class="absolute bottom-4 right-4">
        <div id="vertical-dial" class="group">
            <!-- Main Button -->
            <button id="vertical-dial-trigger" class="flex items-center justify-center w-14 h-14 rounded-full bg-purple-600 text-white shadow-lg hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-500 transition-transform duration-300 z-10">
                <i id="vertical-dial-icon" class="ri-add-line text-2xl transition-transform duration-300"></i>
            </button>
            
            <!-- Speed Dial Options - Hidden by default -->
            <div id="vertical-dial-options" class="absolute bottom-16 right-2 mb-2 hidden">
                <div class="flex flex-col-reverse items-center space-y-reverse space-y-2">
                    <!-- Option 1 -->
                    <button class="flex items-center justify-center w-10 h-10 rounded-full bg-blue-500 text-white shadow-lg hover:bg-blue-600 opacity-0 animate-scale-in delay-1">
                        <i class="ri-camera-line"></i>
                    </button>
                    
                    <!-- Option 2 -->
                    <button class="flex items-center justify-center w-10 h-10 rounded-full bg-green-500 text-white shadow-lg hover:bg-green-600 opacity-0 animate-scale-in delay-2">
                        <i class="ri-image-line"></i>
                    </button>
                    
                    <!-- Option 3 -->
                    <button class="flex items-center justify-center w-10 h-10 rounded-full bg-yellow-500 text-white shadow-lg hover:bg-yellow-600 opacity-0 animate-scale-in delay-3">
                        <i class="ri-file-line"></i>
                    </button>
                    
                    <!-- Option 4 -->
                    <button class="flex items-center justify-center w-10 h-10 rounded-full bg-pink-500 text-white shadow-lg hover:bg-pink-600 opacity-0 animate-scale-in delay-4">
                        <i class="ri-attachment-line"></i>
                    </button>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- JavaScript for Animation -->
<script>
    const verticalDialTrigger = document.getElementById('vertical-dial-trigger');
    const verticalDialOptions = document.getElementById('vertical-dial-options');
    const verticalDialIcon = document.getElementById('vertical-dial-icon');
    let verticalDialOpen = false;
    
    verticalDialTrigger.addEventListener('click', () => {
        verticalDialOpen = !verticalDialOpen;
        
        if (verticalDialOpen) {
            verticalDialOptions.classList.remove('hidden');
            verticalDialIcon.classList.add('rotate-45');
            
            // Reset animations
            const buttons = verticalDialOptions.querySelectorAll('button');
            buttons.forEach(button => {
                button.style.opacity = '0';
                void button.offsetWidth; // Force reflow for animation restart
                button.style.opacity = ''; // Remove inline style to let CSS animation take over
            });
        } else {
            verticalDialOptions.classList.add('hidden');
            verticalDialIcon.classList.remove('rotate-45');
        }
    });
</script>
```

## Example 3: Speed Dial with Text Labels
```html
<div id="labeled-dial" class="group">
    <!-- Main Button -->
    <button id="labeled-dial-trigger" class="flex items-center justify-center w-16 h-16 rounded-full bg-blue-600 text-white shadow-lg hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition-transform duration-300">
        <i id="labeled-dial-icon" class="ri-add-line text-3xl transition-transform duration-300"></i>
    </button>
    
    <!-- Speed Dial Options -->
    <div id="labeled-dial-options" class="absolute bottom-full right-0 mb-4 hidden">
        <div class="flex flex-col-reverse items-end space-y-reverse space-y-4">
            <!-- Option 1 -->
            <div class="flex items-center animate-slide-in opacity-0 delay-1">
                <div class="mr-3 px-4 py-2 bg-white rounded-lg shadow-md">
                    <span class="text-gray-900 whitespace-nowrap font-medium">Create Post</span>
                </div>
                <button class="flex items-center justify-center w-12 h-12 rounded-full bg-red-600 text-white shadow-lg hover:bg-red-700">
                    <i class="ri-article-line text-xl"></i>
                </button>
            </div>
            
            <!-- Option 2 -->
            <div class="flex items-center animate-slide-in opacity-0 delay-2">
                <div class="mr-3 px-4 py-2 bg-white rounded-lg shadow-md">
                    <span class="text-gray-900 whitespace-nowrap font-medium">Upload Photo</span>
                </div>
                <button class="flex items-center justify-center w-12 h-12 rounded-full bg-green-600 text-white shadow-lg hover:bg-green-700">
                    <i class="ri-image-add-line text-xl"></i>
                </button>
            </div>
            
            <!-- Additional options... -->
        </div>
    </div>
</div>
```

## Example 4: Speed Dial with Backdrop
```html
<div class="absolute inset-0">
    <!-- Backdrop - Hidden by default -->
    <div id="backdrop-overlay" class="absolute inset-0 bg-black bg-opacity-0 hidden transition-opacity duration-200"></div>
    
    <div class="absolute bottom-4 right-4">
        <div id="backdrop-dial" class="relative">
            <!-- Main Button -->
            <button id="backdrop-dial-trigger" class="flex items-center justify-center w-14 h-14 rounded-full bg-blue-600 text-white shadow-lg hover:bg-blue-700 focus:outline-none z-10">
                <i id="backdrop-dial-icon" class="ri-add-line text-2xl transition-transform duration-300"></i>
            </button>
            
            <!-- Speed Dial Options -->
            <div id="backdrop-dial-options" class="absolute bottom-16 right-0 mb-2 hidden z-20">
                <div class="flex flex-col-reverse items-center space-y-reverse space-y-3">
                    <!-- Option 1 -->
                    <div class="flex items-center">
                        <span class="bg-gray-800 text-white text-sm px-3 py-1 rounded-md mr-2">Message</span>
                        <button class="flex items-center justify-center w-12 h-12 rounded-full bg-green-500 text-white shadow-lg hover:bg-green-600">
                            <i class="ri-message-3-line text-lg"></i>
                        </button>
                    </div>
                    
                    <!-- Additional options... -->
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 5: Material Design Style Speed Dial
```html
<div id="material-dial" class="relative">
    <!-- Smaller Buttons First (shown when expanded) -->
    <div id="material-dial-options" class="hidden">
        <!-- Button 1 -->
        <div class="absolute -top-24 -translate-x-1/2 left-1/2 transform opacity-0 transition-all duration-200 ease-in-out" id="material-option-1">
            <button class="p-0 w-11 h-11 bg-yellow-500 rounded-full hover:bg-yellow-600 active:shadow-lg mb-2 shadow transition ease-in duration-200 focus:outline-none">
                <i class="ri-attachment-2 text-white text-xl"></i>
            </button>
            <span class="text-xs text-center block text-gray-500 mt-1">Attach</span>
        </div>
        
        <!-- Button 2 -->
        <div class="absolute -top-24 -left-16 transform opacity-0 transition-all duration-200 ease-in-out" id="material-option-2">
            <button class="p-0 w-11 h-11 bg-green-500 rounded-full hover:bg-green-600 active:shadow-lg mb-2 shadow transition ease-in duration-200 focus:outline-none">
                <i class="ri-image-add-line text-white text-xl"></i>
            </button>
            <span class="text-xs text-center block text-gray-500 mt-1">Photo</span>
        </div>
        
        <!-- Button 3 -->
        <div class="absolute -top-24 -right-16 transform opacity-0 transition-all duration-200 ease-in-out" id="material-option-3">
            <button class="p-0 w-11 h-11 bg-blue-500 rounded-full hover:bg-blue-600 active:shadow-lg mb-2 shadow transition ease-in duration-200 focus:outline-none">
                <i class="ri-text text-white text-xl"></i>
            </button>
            <span class="text-xs text-center block text-gray-500 mt-1">Text</span>
        </div>
    </div>
    
    <!-- Main, larger button -->
    <div class="relative">
        <button id="material-dial-trigger" class="p-0 w-16 h-16 bg-pink-600 rounded-full hover:bg-pink-700 active:shadow-lg shadow transition ease-in duration-200 focus:outline-none">
            <i id="material-dial-icon" class="ri-add-line text-white text-3xl transition-transform duration-300"></i>
        </button>
    </div>
</div>
```
