# Mega Menu Component Examples

## Example 1: Basic Mega Menu

```html
<!-- Navbar container -->
<div class="bg-white border-b">
    <div class="flex items-center justify-between px-6 py-3">
        <div class="flex items-center space-x-8">
            <!-- Logo -->
            <a href="#" class="text-2xl font-bold text-blue-600">
                <i class="ri-planet-line"></i> CompanyName
            </a>
            
            <!-- Nav items -->
            <nav class="hidden md:flex items-center space-x-1">
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-blue-600">Home</a>
                
                <!-- Mega menu trigger -->
                <div class="relative menu-hover">
                    <button class="px-3 py-2 text-gray-700 hover:text-blue-600 flex items-center">
                        Products
                        <i class="ri-arrow-down-s-line ml-1"></i>
                    </button>
                    
                    <!-- Mega menu content -->
                    <div class="mega-menu absolute left-0 w-screen max-w-4xl p-6 bg-white rounded-lg shadow-xl border top-full z-50">
                        <div class="grid grid-cols-3 gap-8">
                            <!-- Column 1 -->
                            <div>
                                <h3 class="text-lg font-semibold text-gray-900 mb-4">Software</h3>
                                <ul class="space-y-3">
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-apps-line mr-2"></i> Web Applications</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-smartphone-line mr-2"></i> Mobile Apps</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-database-2-line mr-2"></i> Database Solutions</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-cloud-line mr-2"></i> Cloud Services</a></li>
                                </ul>
                            </div>
                            
                            <!-- Column 2 -->
                            <div>
                                <h3 class="text-lg font-semibold text-gray-900 mb-4">Services</h3>
                                <ul class="space-y-3">
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-code-s-slash-line mr-2"></i> Custom Development</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-user-settings-line mr-2"></i> Consulting</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-tools-line mr-2"></i> Maintenance</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-blue-600 flex items-center"><i class="ri-customer-service-line mr-2"></i> Support</a></li>
                                </ul>
                            </div>
                            
                            <!-- Column 3 -->
                            <div>
                                <h3 class="text-lg font-semibold text-gray-900 mb-4">Resources</h3>
                                <div class="bg-gray-50 rounded-lg p-4">
                                    <p class="text-gray-600 mb-2">Check out our latest case studies</p>
                                    <a href="#" class="block text-blue-600 hover:text-blue-800 font-medium">
                                        Learn more <i class="ri-arrow-right-line inline-block"></i>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-blue-600">About</a>
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-blue-600">Contact</a>
            </nav>
        </div>
        
        <!-- Right action buttons -->
        <div class="flex items-center space-x-3">
            <button class="px-3 py-2 text-gray-700 hover:text-blue-600">
                <i class="ri-search-line text-lg"></i>
            </button>
            <button class="px-3 py-2 text-gray-700 hover:text-blue-600">
                <i class="ri-user-line text-lg"></i>
            </button>
        </div>
    </div>
</div>
```

## Example 2: E-commerce Mega Menu

```html
<!-- Navbar container -->
<div class="bg-gray-900 text-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between h-16">
            <div class="flex items-center space-x-8">
                <!-- Logo -->
                <div class="flex-shrink-0">
                    <a href="#" class="flex items-center">
                        <i class="ri-shopping-bag-line text-2xl text-amber-400"></i>
                        <span class="ml-2 text-lg font-bold">ShopMart</span>
                    </a>
                </div>
                
                <!-- Nav items -->
                <nav class="hidden md:block">
                    <div class="flex items-baseline space-x-1">
                        <a href="#" class="px-3 py-2 text-gray-300 hover:text-white">Home</a>
                        
                        <!-- Mega menu trigger -->
                        <div class="relative menu-hover">
                            <button class="px-3 py-2 text-amber-400 font-medium flex items-center">
                                Shop Categories
                                <i class="ri-arrow-down-s-line ml-1"></i>
                            </button>
                            
                            <!-- Mega menu content -->
                            <div class="mega-menu absolute left-0 w-screen max-w-6xl bg-white rounded-lg shadow-xl text-gray-900 top-full z-50">
                                <div class="grid grid-cols-5 gap-0">
                                    <!-- Category column -->
                                    <div class="bg-gray-100 p-6 rounded-l-lg">
                                        <h3 class="font-bold text-gray-800 mb-4 uppercase text-sm tracking-wider">Browse Categories</h3>
                                        <ul class="space-y-2">
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Electronics</a></li>
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Clothing</a></li>
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Home & Garden</a></li>
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Sports & Outdoors</a></li>
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Toys & Games</a></li>
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Beauty & Personal Care</a></li>
                                            <li><a href="#" class="block py-1 text-gray-700 hover:text-amber-600 font-medium">Books & Media</a></li>
                                        </ul>
                                        <a href="#" class="mt-4 inline-block text-amber-600 hover:underline text-sm font-medium">View All Categories</a>
                                    </div>
                                    
                                    <!-- Featured content -->
                                    <div class="col-span-4 grid grid-cols-4 gap-6 p-6">
                                        <!-- Featured categories -->
                                        <div>
                                            <h4 class="font-semibold text-gray-900 mb-3">Electronics</h4>
                                            <ul class="space-y-2">
                                                <li><a href="#" class="text-gray-600 hover:text-amber-600">Smartphones</a></li>
                                                <li><a href="#" class="text-gray-600 hover:text-amber-600">Laptops</a></li>
                                                <li><a href="#" class="text-gray-600 hover:text-amber-600">Headphones</a></li>
                                                <li><a href="#" class="text-gray-600 hover:text-amber-600">Cameras</a></li>
                                                <li><a href="#" class="text-gray-600 hover:text-amber-600">Smart Watches</a></li>
                                            </ul>
                                        </div>
                                        
                                        <!-- More categories and featured deals... -->
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </nav>
            </div>
        </div>
    </div>
</div>
```

## Example 3: Mega Menu with Images

```html
<!-- Navbar container -->
<div class="bg-white border-b">
    <div class="max-w-7xl mx-auto px-4">
        <div class="flex items-center justify-between h-20">
            <!-- Logo -->
            <div class="flex-shrink-0">
                <a href="#" class="text-2xl font-bold text-indigo-700">
                    <i class="ri-camera-lens-line"></i> TravelWorld
                </a>
            </div>
            
            <!-- Nav items -->
            <nav class="hidden md:flex items-center space-x-4">
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-indigo-700">Home</a>
                
                <!-- Mega menu trigger -->
                <div class="relative menu-hover">
                    <button class="group px-3 py-2 text-gray-700 hover:text-indigo-700 flex items-center font-medium">
                        Destinations
                        <i class="ri-arrow-down-s-line ml-1 group-hover:rotate-180 transition-transform duration-200"></i>
                    </button>
                    
                    <!-- Mega menu content -->
                    <div class="mega-menu absolute left-0 w-screen max-w-6xl bg-white rounded-lg shadow-xl border top-full z-50">
                        <div class="grid grid-cols-4 gap-6 p-8">
                            <!-- Column 1: Popular Destinations -->
                            <div>
                                <h3 class="text-lg font-semibold text-gray-900 mb-4 pb-2 border-b">Popular Destinations</h3>
                                <ul class="space-y-3">
                                    <li><a href="#" class="text-gray-600 hover:text-indigo-700 flex items-center"><i class="ri-map-pin-line mr-2"></i> Paris, France</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-indigo-700 flex items-center"><i class="ri-map-pin-line mr-2"></i> Tokyo, Japan</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-indigo-700 flex items-center"><i class="ri-map-pin-line mr-2"></i> New York, USA</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-indigo-700 flex items-center"><i class="ri-map-pin-line mr-2"></i> Rome, Italy</a></li>
                                    <li><a href="#" class="text-gray-600 hover:text-indigo-700 flex items-center"><i class="ri-map-pin-line mr-2"></i> Bangkok, Thailand</a></li>
                                </ul>
                            </div>
                            
                            <!-- Columns 2 and Featured Destinations with Images... -->
                        </div>
                        
                        <!-- Bottom CTA bar -->
                        <div class="bg-gray-50 p-6 flex items-center justify-between rounded-b-lg">
                            <p class="text-gray-700"><strong>Special offer:</strong> Get 15% off on your first booking</p>
                            <a href="#" class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700 transition-colors">Explore All Destinations</a>
                        </div>
                    </div>
                </div>
            </nav>
        </div>
    </div>
</div>
```

## Example 4: Full Screen Mega Menu

```html
<!-- Navbar container -->
<div class="bg-gray-800 text-white">
    <div class="max-w-7xl mx-auto px-4">
        <div class="flex items-center justify-between h-16">
            <!-- Logo -->
            <div class="flex-shrink-0">
                <a href="#" class="text-xl font-bold text-white">
                    <i class="ri-code-box-line"></i> TechSolutions
                </a>
            </div>
            
            <!-- Navigation -->
            <nav class="hidden md:flex items-center space-x-4">
                <a href="#" class="px-3 py-2 text-gray-300 hover:text-white">Home</a>
                
                <!-- JS controlled mega menu -->
                <div class="relative" id="megaMenuContainer">
                    <button id="megaMenuTrigger" class="group px-3 py-2 text-gray-300 hover:text-white flex items-center">
                        Services
                        <i class="ri-arrow-down-s-line ml-1"></i>
                    </button>
                </div>
                
                <a href="#" class="px-3 py-2 text-gray-300 hover:text-white">About</a>
                <a href="#" class="px-3 py-2 text-gray-300 hover:text-white">Blog</a>
                <a href="#" class="px-3 py-2 text-gray-300 hover:text-white">Contact</a>
            </nav>
        </div>
    </div>
</div>

<!-- Full screen mega menu -->
<div id="fullScreenMegaMenu" class="mega-menu-animated fixed inset-0 bg-white z-50 overflow-y-auto" style="display:none;">
    <div class="max-w-7xl mx-auto px-4 py-12">
        <!-- Header with close button -->
        <div class="flex justify-between items-center mb-12">
            <h2 class="text-3xl font-bold text-gray-900">Our Services</h2>
            <button id="closeMegaMenu" class="text-gray-500 hover:text-gray-900">
                <i class="ri-close-line text-3xl"></i>
            </button>
        </div>
        
        <!-- Mega menu content -->
        <div class="grid grid-cols-3 gap-8">
            <!-- Service Categories... -->
        </div>
        
        <!-- Featured case studies -->
        <div class="mt-12 pt-12 border-t">
            <h3 class="text-xl font-bold text-gray-900 mb-6">Featured Case Studies</h3>
            <div class="grid grid-cols-3 gap-6">
                <!-- Case Study Items... -->
            </div>
        </div>
    </div>
</div>

<script>
    // Demo functionality for the full-screen mega menu
    document.addEventListener('DOMContentLoaded', function() {
        const megaMenuTrigger = document.getElementById('megaMenuTrigger');
        const closeMegaMenu = document.getElementById('closeMegaMenu');
        const fullScreenMegaMenu = document.getElementById('fullScreenMegaMenu');
        
        function openMegaMenu() {
            fullScreenMegaMenu.style.display = 'block';
            setTimeout(() => {
                document.body.classList.add('mega-active');
            }, 10);
        }
        
        function closeMegaMenuFn() {
            document.body.classList.remove('mega-active');
            setTimeout(() => {
                fullScreenMegaMenu.style.display = 'none';
            }, 300);
        }
        
        if (megaMenuTrigger) {
            megaMenuTrigger.addEventListener('click', openMegaMenu);
        }
        
        if (closeMegaMenu) {
            closeMegaMenu.addEventListener('click', closeMegaMenuFn);
        }
    });
</script>
```

## Example 5: Mobile Friendly Mega Menu

```html
<!-- Navbar container -->
<div class="bg-white border-b">
    <div class="max-w-7xl mx-auto">
        <div class="flex items-center justify-between px-4 py-3 sm:p-0">
            <!-- Logo -->
            <div class="flex items-center">
                <a href="#" class="text-xl font-bold text-emerald-600">
                    <i class="ri-leaf-line"></i> GreenLife
                </a>
            </div>
            
            <!-- Mobile menu button -->
            <div class="sm:hidden">
                <button type="button" id="mobileMenuButton" class="text-gray-500 hover:text-gray-700 focus:outline-none">
                    <i class="ri-menu-line text-2xl"></i>
                </button>
            </div>
            
            <!-- Desktop menu -->
            <nav class="hidden sm:flex items-center space-x-4">
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-emerald-600">Home</a>
                
                <!-- Mega menu trigger (desktop) -->
                <div class="relative menu-hover">
                    <button class="px-3 py-2 text-gray-700 hover:text-emerald-600 flex items-center">
                        Products
                        <i class="ri-arrow-down-s-line ml-1"></i>
                    </button>
                    
                    <!-- Mega menu (desktop) -->
                    <div class="mega-menu absolute left-0 w-screen max-w-5xl bg-white shadow-xl rounded-lg border p-6 top-full z-50">
                        <!-- Desktop menu content... -->
                    </div>
                </div>
                
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-emerald-600">Blog</a>
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-emerald-600">About</a>
                <a href="#" class="px-3 py-2 text-gray-700 hover:text-emerald-600">Contact</a>
            </nav>
        </div>
    </div>
</div>

<!-- Mobile menu (Initially hidden) -->
<div id="mobileMenu" class="sm:hidden bg-white shadow-lg hidden">
    <div class="px-2 pt-2 pb-3 space-y-1">
        <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-emerald-600 hover:bg-gray-50">Home</a>
        
        <!-- Mobile accordion menu -->
        <div class="relative">
            <button id="mobileProductsButton" class="w-full flex justify-between items-center px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-emerald-600 hover:bg-gray-50">
                Products
                <i class="ri-arrow-down-s-line ml-1"></i>
            </button>
            
            <!-- Mobile submenu (initially hidden) -->
            <div id="mobileProductsSubmenu" class="hidden px-4 py-2 bg-gray-50 rounded-md mt-1">
                <!-- Mobile submenu content... -->
            </div>
        </div>
        
        <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-emerald-600 hover:bg-gray-50">Blog</a>
        <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-emerald-600 hover:bg-gray-50">About</a>
        <a href="#" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-emerald-600 hover:bg-gray-50">Contact</a>
    </div>
</div>

<script>
    // Mobile menu functionality
    document.addEventListener('DOMContentLoaded', function() {
        const mobileMenuButton = document.getElementById('mobileMenuButton');
        const mobileMenu = document.getElementById('mobileMenu');
        const mobileProductsButton = document.getElementById('mobileProductsButton');
        const mobileProductsSubmenu = document.getElementById('mobileProductsSubmenu');
        
        function toggleMobileMenu() {
            mobileMenu.classList.toggle('hidden');
        }
        
        function toggleProductsSubmenu() {
            mobileProductsSubmenu.classList.toggle('hidden');
            mobileProductsButton.querySelector('i').classList.toggle('rotate-180');
        }
        
        if (mobileMenuButton) {
            mobileMenuButton.addEventListener('click', toggleMobileMenu);
        }
        
        if (mobileProductsButton) {
            mobileProductsButton.addEventListener('click', toggleProductsSubmenu);
        }
    });
</script>
```

Add the following CSS to make the mega menu work with the hover effect:

```css
.mega-menu {
    opacity: 0;
    visibility: hidden;
    transform: translateY(15px);
    transition: all 0.2s ease-in-out;
}
.menu-hover:hover .mega-menu {
    opacity: 1;
    visibility: visible;
    transform: translateY(0);
}
.mega-menu-animated {
    display: none;
    transform: translateY(-10px);
    transition: all 0.3s ease;
}
.mega-active .mega-menu-animated {
    display: block;
    transform: translateY(0);
}
```
