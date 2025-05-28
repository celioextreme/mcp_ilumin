# Popover Examples with Tailwind CSS

## Example 1: Basic Popovers
```html
<!-- Top Popover -->
<div class="relative inline-block" x-data="{ open: false }">
    <button 
        class="bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-md focus:outline-none"
        onClick="togglePopover(this, 'popover-top')"
    >
        <i class="ri-arrow-up-line mr-1"></i> Popover on Top
    </button>
    <div id="popover-top" class="popover absolute bottom-full left-1/2 transform -translate-x-1/2 -translate-y-2 mb-2 w-64 bg-white rounded-md shadow-lg p-4 z-10">
        <div class="popover-arrow bg-white bottom-0 left-1/2 transform -translate-x-1/2 translate-y-1/2"></div>
        <h3 class="font-medium text-gray-900 mb-1">Popover Title</h3>
        <p class="text-sm text-gray-600">This is a basic popover that appears on the top of the trigger element.</p>
    </div>
</div>
```

## Example 2: Styled Popovers with Icons
```html
<!-- Info Popover -->
<div class="relative inline-block">
    <button 
        class="flex items-center bg-blue-100 text-blue-800 hover:bg-blue-200 px-4 py-2 rounded-lg focus:outline-none transition-all"
        onClick="togglePopover(this, 'popover-info')"
    >
        <i class="ri-information-line text-xl mr-2"></i> Information
    </button>
    <div id="popover-info" class="popover absolute bottom-full left-1/2 transform -translate-x-1/2 -translate-y-2 mb-3 w-72 bg-blue-50 border border-blue-200 rounded-lg shadow-lg p-4 z-10">
        <div class="popover-arrow bg-blue-50 bottom-0 left-1/2 transform -translate-x-1/2 translate-y-1/2 border-r border-b border-blue-200"></div>
        <div class="flex items-start">
            <i class="ri-information-fill text-2xl text-blue-500 mr-3 mt-1"></i>
            <div>
                <h3 class="font-semibold text-blue-900 mb-1">Important Information</h3>
                <p class="text-sm text-blue-700">This popover provides additional information and context for the current section.</p>
            </div>
        </div>
        <div class="mt-2 pt-2 border-t border-blue-200 text-xs text-blue-600">Last updated: Today</div>
    </div>
</div>
```

## Example 3: Interactive Popover with Forms
```html
<!-- Login Popover -->
<div class="relative inline-block">
    <button 
        class="bg-indigo-600 hover:bg-indigo-700 text-white px-5 py-2.5 rounded-lg focus:outline-none transition-all"
        onClick="togglePopover(this, 'popover-login')"
    >
        <i class="ri-login-box-line mr-2"></i> Quick Login
    </button>
    <div id="popover-login" class="popover absolute top-full left-1/2 transform -translate-x-1/2 translate-y-3 mt-1 w-80 bg-white rounded-lg shadow-xl p-4 z-10 border border-gray-200">
        <div class="popover-arrow bg-white top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2 border-t border-l border-gray-200"></div>
        <div class="text-center mb-3">
            <h3 class="font-bold text-lg text-gray-800">Sign In</h3>
            <p class="text-xs text-gray-500">Access your account quickly</p>
        </div>
        <form class="space-y-3">
            <!-- Form content here -->
        </form>
    </div>
</div>
```

## Example 4: Popover with Rich Media Content
```html
<!-- Product Popover -->
<div class="relative inline-block">
    <button 
        class="bg-teal-600 hover:bg-teal-700 text-white px-5 py-2.5 rounded-lg focus:outline-none transition-all"
        onClick="togglePopover(this, 'popover-product')"
    >
        <i class="ri-shopping-bag-line mr-2"></i> Product Details
    </button>
    <div id="popover-product" class="popover absolute top-full left-1/2 transform -translate-x-1/2 translate-y-3 mt-1 w-80 bg-white rounded-lg shadow-xl z-10 overflow-hidden border border-gray-200">
        <div class="bg-gray-100 p-3 flex items-center justify-between border-b">
            <h3 class="font-medium text-gray-800">Premium Headphones</h3>
            <div class="flex items-center">
                <span class="text-sm font-semibold text-teal-600 mr-1">$129.99</span>
                <span class="text-xs text-gray-500 line-through">$149.99</span>
            </div>
        </div>
        <!-- Product content here -->
    </div>
</div>
```

## Example 5: Interactive Popovers with Animations
```html
<!-- Notification Popover -->
<div class="relative inline-block">
    <button 
        class="relative flex items-center bg-red-600 hover:bg-red-700 text-white px-5 py-2.5 rounded-lg focus:outline-none transition-all"
        onClick="togglePopover(this, 'popover-notifications', true)"
    >
        <i class="ri-notification-3-line mr-2"></i> 
        <span>Notifications</span>
        <span class="ml-1.5 flex h-5 w-5 items-center justify-center rounded-full bg-red-100 text-xs text-red-800">3</span>
    </button>
    <div id="popover-notifications" class="popover absolute top-full right-0 translate-y-3 mt-1 w-80 bg-white rounded-lg shadow-xl z-10 overflow-hidden border border-gray-200">
        <!-- Notification content here -->
    </div>
</div>
```

## JavaScript for Popover Functionality
```javascript
// Function to toggle popover visibility
function togglePopover(button, popoverId, clickOutside = false) {
    const popover = document.getElementById(popoverId);
    
    // Toggle show class
    if (popover.classList.contains('show')) {
        popover.classList.remove('show');
    } else {
        // Close any open popovers first
        document.querySelectorAll('.popover.show').forEach(el => {
            el.classList.remove('show');
        });
        
        popover.classList.add('show');
        
        // Add click outside event listener if needed
        if (clickOutside) {
            setTimeout(() => {
                window.addEventListener('click', function closePopover(e) {
                    if (!popover.contains(e.target) && e.target !== button) {
                        popover.classList.remove('show');
                        window.removeEventListener('click', closePopover);
                    }
                });
            }, 10);
        }
    }
}
```

## CSS for Popover Animations
```css
.popover {
    visibility: hidden;
    opacity: 0;
    transition: visibility 0s, opacity 0.3s ease;
}
.popover.show {
    visibility: visible;
    opacity: 1;
}
.popover-arrow {
    position: absolute;
    width: 10px;
    height: 10px;
    background: inherit;
    visibility: hidden;
}
.popover-arrow::before {
    content: '';
    position: absolute;
    width: 10px;
    height: 10px;
    background: inherit;
    visibility: visible;
    transform: rotate(45deg);
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
}

.animate-fadeIn {
    animation: fadeIn 0.3s ease-out forwards;
}
```
