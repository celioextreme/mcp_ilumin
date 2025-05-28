# Device Mockups Component Examples

## Example 1: Basic Phone Mockup
```html
<div class="device bg-black w-64 h-[500px] device-shadow p-3">
    <div class="device-notch"></div>
    <div class="bg-white h-full w-full rounded-3xl overflow-hidden relative">
        <img src="https://via.placeholder.com/400x800/3b82f6/FFFFFF?text=App+Screen" alt="App Screenshot" class="w-full h-full object-cover">
        
        <!-- Sample content overlay -->
        <div class="absolute inset-0 flex flex-col">
            <!-- Status bar -->
            <div class="h-10 bg-blue-600 flex items-center justify-between px-4">
                <span class="text-white text-xs font-semibold">9:41 AM</span>
                <div class="flex items-center space-x-1">
                    <i class="ri-signal-wifi-fill text-white text-xs"></i>
                    <i class="ri-battery-fill text-white text-xs"></i>
                </div>
            </div>
            
            <!-- Content -->
            <div class="flex-grow flex flex-col p-4">
                <h3 class="text-white text-lg font-bold mb-2">My Mobile App</h3>
                <div class="bg-white/20 backdrop-blur-sm rounded-lg p-4 mb-4">
                    <p class="text-white text-sm">Welcome to your new application!</p>
                </div>
                
                <div class="mt-auto flex justify-between">
                    <div class="w-12 h-12 rounded-full bg-white/20 flex items-center justify-center">
                        <i class="ri-home-line text-white"></i>
                    </div>
                    <div class="w-12 h-12 rounded-full bg-white/20 flex items-center justify-center">
                        <i class="ri-search-line text-white"></i>
                    </div>
                    <div class="w-12 h-12 rounded-full bg-white/20 flex items-center justify-center">
                        <i class="ri-user-line text-white"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
.device-shadow {
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1), 0 5px 15px rgba(0, 0, 0, 0.07);
}

.device {
    position: relative;
    border-radius: 36px;
    overflow: hidden;
}

.device-notch {
    position: absolute;
    width: 150px;
    height: 30px;
    background-color: #000;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    border-bottom-left-radius: 18px;
    border-bottom-right-radius: 18px;
    z-index: 2;
}
</style>
```

## Example 2: Laptop Mockup
```html
<div class="laptop-mockup">
    <!-- Screen -->
    <div class="bg-gray-800 rounded-t-lg p-2 device-shadow">
        <div class="bg-white rounded-md overflow-hidden">
            <img src="https://via.placeholder.com/1200x800/f3f4f6/4b5563?text=Website+Screenshot" alt="Website Screenshot" class="w-full">
            
            <!-- Sample content overlay -->
            <div class="absolute inset-0 m-2 flex flex-col pointer-events-none">
                <!-- Browser chrome -->
                <div class="h-8 bg-gray-100 border-b border-gray-200 flex items-center px-3 space-x-2">
                    <div class="flex space-x-1.5">
                        <div class="w-3 h-3 rounded-full bg-red-500"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                        <div class="w-3 h-3 rounded-full bg-green-500"></div>
                    </div>
                    <div class="flex-grow mx-2">
                        <div class="bg-white h-5 w-full rounded-md border border-gray-300 flex items-center px-3">
                            <span class="text-gray-500 text-xs truncate">https://example.com</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Base/Keyboard -->
    <div class="laptop-keyboard rounded-b-lg"></div>
</div>

<style>
.laptop-keyboard {
    height: 40px;
    background: linear-gradient(to bottom, #f5f5f7, #e2e2e7);
    position: relative;
}

.laptop-keyboard::after {
    content: '';
    position: absolute;
    width: 30%;
    height: 4px;
    background-color: #d1d1d6;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    border-radius: 2px;
}
</style>
```

## Example 3: Multi-Device Mockup
```html
<div class="flex flex-col md:flex-row items-center justify-center gap-8">
    <!-- Desktop -->
    <div class="bg-gray-800 rounded-lg p-3 device-shadow">
        <div class="rounded overflow-hidden w-80 h-56">
            <img src="https://via.placeholder.com/800x600/6366f1/ffffff?text=Desktop+View" alt="Desktop View" class="w-full h-full object-cover">
        </div>
        <div class="h-3 w-20 bg-gray-700 mx-auto mt-1 rounded-b"></div>
    </div>
    
    <!-- Tablet -->
    <div class="bg-gray-800 rounded-xl p-2 device-shadow">
        <div class="rounded overflow-hidden w-48 h-64">
            <img src="https://via.placeholder.com/600x800/6366f1/ffffff?text=Tablet+View" alt="Tablet View" class="w-full h-full object-cover">
        </div>
        <div class="h-3 w-3 bg-gray-700 mx-auto mt-2 rounded-full"></div>
    </div>
    
    <!-- Phone -->
    <div class="bg-gray-800 rounded-xl p-1 device-shadow">
        <div class="rounded overflow-hidden w-24 h-48">
            <img src="https://via.placeholder.com/400x800/6366f1/ffffff?text=Mobile+View" alt="Mobile View" class="w-full h-full object-cover">
        </div>
        <div class="h-2 w-8 bg-gray-700 mx-auto mt-1 rounded"></div>
    </div>
</div>
```

## Example 4: iMac Mockup
```html
<div class="imac-mockup">
    <!-- Screen -->
    <div class="bg-gray-200 rounded-t-xl p-3 device-shadow">
        <div class="bg-black rounded-lg overflow-hidden">
            <div class="relative">
                <img src="https://via.placeholder.com/1800x1200/2563eb/ffffff?text=Desktop+App" alt="Desktop App" class="w-full h-[400px] object-cover">
                
                <!-- Sample content overlay -->
                <div class="absolute inset-0 flex flex-col">
                    <!-- Menu bar -->
                    <div class="h-8 bg-gray-800/80 backdrop-blur flex items-center px-4">
                        <div class="flex space-x-1.5">
                            <div class="w-3 h-3 rounded-full bg-red-500"></div>
                            <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                            <div class="w-3 h-3 rounded-full bg-green-500"></div>
                        </div>
                        <div class="flex-grow"></div>
                        <div class="flex space-x-4 text-white text-xs">
                            <span>File</span>
                            <span>Edit</span>
                            <span>View</span>
                            <span>Help</span>
                        </div>
                        <div class="flex-grow"></div>
                        <div class="text-white text-xs">
                            <span>10:42 AM</span>
                        </div>
                    </div>
                    
                    <!-- App content -->
                    <div class="flex-grow grid grid-cols-12 gap-4 p-4">
                        <div class="col-span-3 bg-white/10 backdrop-blur-sm rounded-lg"></div>
                        <div class="col-span-9 bg-white/10 backdrop-blur-sm rounded-lg"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Stand -->
    <div class="imac-stand"></div>
    <div class="imac-foot"></div>
</div>

<style>
.imac-stand {
    height: 60px;
    width: 120px;
    background: linear-gradient(to bottom, #e2e2e7, #f5f5f7);
    margin: 0 auto;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
}

.imac-foot {
    height: 20px;
    width: 200px;
    background: #e2e2e7;
    margin: 0 auto;
    border-bottom-left-radius: 50%;
    border-bottom-right-radius: 50%;
}
</style>
```

## Example 5: Interactive Device Preview
```html
<!-- Device Selection Tabs -->
<div class="flex space-x-2 mb-6">
    <button 
        class="px-4 py-2 rounded-md bg-blue-600 text-white font-medium shadow-md device-btn active" 
        data-device="phone">
        <i class="ri-smartphone-line mr-2"></i>Phone
    </button>
    <button 
        class="px-4 py-2 rounded-md bg-gray-200 text-gray-700 font-medium shadow-md device-btn" 
        data-device="tablet">
        <i class="ri-tablet-line mr-2"></i>Tablet
    </button>
    <button 
        class="px-4 py-2 rounded-md bg-gray-200 text-gray-700 font-medium shadow-md device-btn" 
        data-device="laptop">
        <i class="ri-macbook-line mr-2"></i>Laptop
    </button>
</div>

<!-- Device Mockups Container -->
<div class="device-preview-container relative h-[500px] w-full flex justify-center">
    <!-- Phone Preview (visible by default) -->
    <div id="phone-preview" class="device-preview absolute">
        <div class="device bg-gray-900 w-64 h-[450px] device-shadow rounded-3xl p-2">
            <!-- Phone content -->
            <!-- ... -->
        </div>
    </div>
    
    <!-- Tablet Preview (hidden by default) -->
    <div id="tablet-preview" class="device-preview absolute hidden">
        <!-- Tablet content -->
        <!-- ... -->
    </div>
    
    <!-- Laptop Preview (hidden by default) -->
    <div id="laptop-preview" class="device-preview absolute hidden">
        <!-- Laptop content -->
        <!-- ... -->
    </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
    // Setup interactive device preview
    const deviceButtons = document.querySelectorAll('.device-btn');
    const devicePreviews = document.querySelectorAll('.device-preview');
    
    deviceButtons.forEach(button => {
        button.addEventListener('click', () => {
            const device = button.getAttribute('data-device');
            
            // Update active button
            deviceButtons.forEach(btn => {
                btn.classList.remove('bg-blue-600', 'text-white');
                btn.classList.add('bg-gray-200', 'text-gray-700');
            });
            button.classList.remove('bg-gray-200', 'text-gray-700');
            button.classList.add('bg-blue-600', 'text-white');
            
            // Show selected device preview
            devicePreviews.forEach(preview => {
                preview.classList.add('hidden');
            });
            
            const targetPreview = document.getElementById(`${device}-preview`);
            targetPreview.classList.remove('hidden');
            targetPreview.classList.add('animate-fadeInUp');
        });
    });
});
</script>

<style>
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.animate-fadeInUp {
    animation: fadeInUp 0.5s ease-out forwards;
}
</style>
```
