# Drawer Component Examples

## Example 1: Basic Drawer - Left Side
```html
<!-- Drawer Overlay -->
<div class="fixed inset-0 bg-black bg-opacity-50 z-10 hidden drawer-overlay" id="drawer1Overlay"></div>

<!-- Drawer -->
<div class="fixed inset-y-0 left-0 w-64 bg-white shadow-lg z-20 transform -translate-x-full drawer" id="drawer1">
    <div class="p-4 border-b border-gray-200 flex items-center justify-between">
        <h2 class="font-semibold text-gray-800">Menu</h2>
        <button class="p-1 rounded-full hover:bg-gray-100 transition-colors" id="closeDrawer1">
            <i class="ri-close-line text-gray-500"></i>
        </button>
    </div>
    <nav class="p-4">
        <ul class="space-y-2">
            <li>
                <a href="#" class="flex items-center p-2 text-gray-700 rounded-md hover:bg-gray-100 transition-colors">
                    <i class="ri-dashboard-line mr-3 text-gray-500"></i>
                    <span>Dashboard</span>
                </a>
            </li>
            <!-- More menu items -->
        </ul>
    </nav>
</div>

<script>
    // Toggle drawer
    document.getElementById('toggleButton').addEventListener('click', () => {
        document.getElementById('drawer1').classList.toggle('-translate-x-full');
        document.getElementById('drawer1Overlay').classList.toggle('hidden');
    });
    
    // Close drawer
    document.getElementById('closeDrawer1').addEventListener('click', () => {
        document.getElementById('drawer1').classList.add('-translate-x-full');
        document.getElementById('drawer1Overlay').classList.add('hidden');
    });
    
    // Click overlay to close
    document.getElementById('drawer1Overlay').addEventListener('click', () => {
        document.getElementById('drawer1').classList.add('-translate-x-full');
        document.getElementById('drawer1Overlay').classList.add('hidden');
    });
</script>
```

## Example 2: Right Side Drawer with Backdrop
```html
<!-- Drawer Overlay -->
<div class="fixed inset-0 bg-black bg-opacity-50 backdrop-blur-sm z-10 hidden drawer-overlay" id="drawer2Overlay"></div>

<!-- Drawer -->
<div class="fixed inset-y-0 right-0 w-72 bg-white shadow-lg z-20 transform translate-x-full drawer" id="drawer2">
    <div class="p-4 border-b border-gray-200 flex items-center justify-between">
        <h2 class="font-semibold text-gray-800">User Settings</h2>
        <button class="p-1 rounded-full hover:bg-gray-100 transition-colors" id="closeDrawer2">
            <i class="ri-close-line text-gray-500"></i>
        </button>
    </div>
    <div class="p-4">
        <div class="flex items-center mb-6">
            <div class="w-12 h-12 rounded-full bg-indigo-100 flex items-center justify-center text-indigo-600 font-semibold">JD</div>
            <div class="ml-3">
                <p class="font-medium text-gray-800">Jane Doe</p>
                <p class="text-xs text-gray-500">jane.doe@example.com</p>
            </div>
        </div>
        <!-- Content -->
    </div>
</div>
```

## Example 3: Bottom Sheet Drawer
```html
<!-- Drawer Overlay -->
<div class="fixed inset-0 bg-black bg-opacity-50 z-10 hidden drawer-overlay" id="drawer3Overlay"></div>

<!-- Bottom Drawer -->
<div class="fixed inset-x-0 bottom-0 bg-white rounded-t-xl shadow-lg z-20 transform translate-y-full drawer" id="drawer3" style="max-height: 90vh; overflow-y: auto;">
    <div class="p-4 border-b border-gray-200">
        <div class="w-12 h-1 bg-gray-300 rounded-full mx-auto mb-2"></div>
        <h2 class="font-semibold text-gray-800 text-center">Share Options</h2>
    </div>
    <div class="p-4">
        <div class="grid grid-cols-4 gap-4 mb-6">
            <div class="flex flex-col items-center">
                <button class="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center text-blue-600 hover:bg-blue-200 transition-colors">
                    <i class="ri-facebook-fill text-xl"></i>
                </button>
                <span class="text-xs text-gray-500 mt-1">Facebook</span>
            </div>
            <!-- More share options -->
        </div>
        <!-- More content -->
    </div>
</div>
```

## Example 4: Drawer with Form
```html
<!-- Drawer Overlay -->
<div class="fixed inset-0 bg-black bg-opacity-50 z-10 hidden drawer-overlay" id="drawer4Overlay"></div>

<!-- Drawer with Form -->
<div class="fixed inset-y-0 right-0 w-96 bg-white shadow-lg z-20 transform translate-x-full drawer" id="drawer4">
    <div class="p-4 border-b border-gray-200 flex items-center justify-between">
        <h2 class="font-semibold text-gray-800">Add New Product</h2>
        <button class="p-1 rounded-full hover:bg-gray-100 transition-colors" id="closeDrawer4">
            <i class="ri-close-line text-gray-500"></i>
        </button>
    </div>
    <div class="p-4 flex flex-col h-full">
        <div class="flex-1 overflow-y-auto">
            <form class="space-y-4">
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Product Name</label>
                    <input type="text" class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:border-indigo-500" placeholder="Enter product name">
                </div>
                <!-- More form fields -->
            </form>
        </div>
        <div class="pt-4 border-t border-gray-200 mt-4">
            <div class="flex space-x-3">
                <button class="flex-1 py-2 bg-gray-100 text-gray-700 rounded-md hover:bg-gray-200 transition-colors">
                    Cancel
                </button>
                <button class="flex-1 py-2 bg-indigo-600 text-white rounded-md hover:bg-indigo-700 transition-colors">
                    Save Product
                </button>
            </div>
        </div>
    </div>
</div>
```

## Example 5: Multi-level Drawer with Nested Navigation
```html
<!-- Drawer Overlay -->
<div class="fixed inset-0 bg-black bg-opacity-50 z-10 hidden drawer-overlay" id="drawer5Overlay"></div>

<!-- Multi-level Drawer -->
<div class="fixed inset-y-0 left-0 w-72 bg-gray-900 text-gray-100 shadow-lg z-20 transform -translate-x-full drawer" id="drawer5">
    <div class="p-4 border-b border-gray-700 flex items-center justify-between">
        <h2 class="font-semibold text-white flex items-center">
            <i class="ri-dashboard-line mr-2"></i>
            Admin Panel
        </h2>
        <button class="p-1 rounded-full hover:bg-gray-800 transition-colors" id="closeDrawer5">
            <i class="ri-close-line text-gray-400"></i>
        </button>
    </div>
    <div class="p-2">
        <div class="mb-4">
            <div class="flex items-center px-3 py-2 text-gray-400 text-xs uppercase font-semibold">
                <span>Main Navigation</span>
            </div>
            <ul class="mt-1">
                <li>
                    <a href="#" class="flex items-center px-3 py-2 text-gray-300 rounded-md hover:bg-gray-800 hover:text-white transition-colors">
                        <i class="ri-home-line mr-3"></i>
                        <span>Dashboard</span>
                    </a>
                </li>
                
                <!-- Expandable Menu Item -->
                <li class="relative">
                    <button class="w-full flex items-center justify-between px-3 py-2 text-gray-300 rounded-md hover:bg-gray-800 hover:text-white transition-colors">
                        <div class="flex items-center">
                            <i class="ri-shopping-bag-line mr-3"></i>
                            <span>Products</span>
                        </div>
                        <i class="ri-arrow-down-s-line"></i>
                    </button>
                    <ul class="pl-10 mt-1 space-y-1">
                        <li>
                            <a href="#" class="block px-3 py-1 text-gray-400 hover:text-gray-100 transition-colors text-sm">
                                All Products
                            </a>
                        </li>
                        <!-- More submenu items -->
                    </ul>
                </li>
                <!-- More menu items -->
            </ul>
        </div>
    </div>
</div>
```

## Drawer CSS Styles
```html
<style>
    .drawer {
        transition: transform 0.3s ease-in-out;
    }
    
    .drawer-overlay {
        transition: opacity 0.3s ease-in-out;
    }
</style>
```
