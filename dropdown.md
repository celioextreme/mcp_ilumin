# Dropdown Component Examples

## Example 1: Basic Dropdown

```html
<div class="flex items-center justify-center">
    <button id="dropdownDefaultButton" data-dropdown-toggle="dropdown" class="text-white bg-blue-600 hover:bg-blue-700 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center" type="button">
        Dropdown Menu
        <i class="ri-arrow-down-s-line ml-2 text-lg"></i>
    </button>
    
    <div id="dropdown" data-dropdown class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44">
        <ul class="py-2 text-sm text-gray-700" aria-labelledby="dropdownDefaultButton">
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Dashboard</a>
            </li>
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Settings</a>
            </li>
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Earnings</a>
            </li>
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Sign out</a>
            </li>
        </ul>
    </div>
</div>
```

## Example 2: Dropdown with Icons

```html
<div class="flex items-center justify-center">
    <button id="dropdownWithIconsButton" data-dropdown-toggle="dropdownWithIcons" class="text-white bg-indigo-600 hover:bg-indigo-700 focus:ring-4 focus:outline-none focus:ring-indigo-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center" type="button">
        Menu with Icons
        <i class="ri-arrow-down-s-line ml-2 text-lg"></i>
    </button>
    
    <div id="dropdownWithIcons" data-dropdown class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-48">
        <ul class="py-2 text-sm text-gray-700" aria-labelledby="dropdownWithIconsButton">
            <li>
                <a href="#" class="flex items-center px-4 py-2 hover:bg-gray-100">
                    <i class="ri-dashboard-line mr-2 text-indigo-600"></i> Dashboard
                </a>
            </li>
            <li>
                <a href="#" class="flex items-center px-4 py-2 hover:bg-gray-100">
                    <i class="ri-settings-4-line mr-2 text-indigo-600"></i> Settings
                </a>
            </li>
            <li>
                <a href="#" class="flex items-center px-4 py-2 hover:bg-gray-100">
                    <i class="ri-wallet-3-line mr-2 text-indigo-600"></i> Earnings
                </a>
            </li>
            <li>
                <a href="#" class="flex items-center px-4 py-2 hover:bg-gray-100">
                    <i class="ri-logout-box-r-line mr-2 text-red-500"></i> Sign out
                </a>
            </li>
        </ul>
    </div>
</div>
```

## Example 3: Dropdown with Divider

```html
<div class="flex items-center justify-center">
    <button id="dropdownDividerButton" data-dropdown-toggle="dropdownDivider" class="text-white bg-green-600 hover:bg-green-700 focus:ring-4 focus:outline-none focus:ring-green-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center" type="button">
        Account Options
        <i class="ri-arrow-down-s-line ml-2 text-lg"></i>
    </button>
    
    <div id="dropdownDivider" data-dropdown class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44">
        <div class="px-4 py-3 text-sm text-gray-900">
            <div class="font-medium">Alex Johnson</div>
            <div class="truncate">alex.johnson@example.com</div>
        </div>
        <ul class="py-2 text-sm text-gray-700" aria-labelledby="dropdownDividerButton">
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Dashboard</a>
            </li>
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Settings</a>
            </li>
            <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100">Earnings</a>
            </li>
        </ul>
        <div class="py-2">
            <a href="#" class="block px-4 py-2 text-sm text-red-600 hover:bg-gray-100">Sign out</a>
        </div>
    </div>
</div>
```

## Example 4: Hover Dropdown

```html
<div class="flex items-center justify-center">
    <div class="relative" data-dropdown-hover="dropdownHover">
        <button class="text-white bg-purple-600 hover:bg-purple-700 focus:ring-4 focus:outline-none focus:ring-purple-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center" type="button">
            Hover to Show
            <i class="ri-arrow-down-s-line ml-2 text-lg"></i>
        </button>
        
        <div id="dropdownHover" data-dropdown class="absolute z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44 mt-1">
            <ul class="py-2 text-sm text-gray-700">
                <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100">Products</a>
                </li>
                <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100">Features</a>
                </li>
                <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100">Solutions</a>
                </li>
                <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100">Resources</a>
                </li>
            </ul>
        </div>
    </div>
</div>
```

## Example 5: Notification Dropdown

```html
<div class="flex items-center justify-center">
    <button id="notificationDropdownButton" data-dropdown-toggle="notificationDropdown" class="relative p-2 text-gray-600 rounded-lg hover:bg-gray-100 focus:ring-4 focus:outline-none focus:ring-blue-300" type="button">
        <span class="absolute inline-flex items-center justify-center w-5 h-5 text-xs font-bold text-white bg-red-500 border-2 border-white rounded-full -top-1 -right-1">3</span>
        <i class="ri-notification-3-line text-2xl"></i>
    </button>
    
    <div id="notificationDropdown" data-dropdown class="z-20 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-80">
        <div class="block px-4 py-2 font-medium text-gray-700 bg-gray-50 rounded-t-lg flex justify-between items-center">
            <span>Notifications</span>
            <span class="bg-blue-100 text-blue-800 text-xs font-medium rounded px-2 py-0.5">3 New</span>
        </div>
        <div class="divide-y divide-gray-100 max-h-80 overflow-y-auto">
            <a href="#" class="flex px-4 py-3 hover:bg-gray-100">
                <div class="flex-shrink-0">
                    <div class="w-11 h-11 rounded-full bg-pink-100 flex items-center justify-center text-pink-500">
                        <i class="ri-message-3-line text-xl"></i>
                    </div>
                </div>
                <div class="w-full pl-3">
                    <div class="text-gray-500 text-sm mb-1.5">New message from <span class="font-semibold text-gray-900">Sarah Johnson</span>: "Hi there, can we schedule a meeting tomorrow?"</div>
                    <div class="text-xs text-blue-600">5 minutes ago</div>
                </div>
            </a>
            <a href="#" class="flex px-4 py-3 hover:bg-gray-100">
                <div class="flex-shrink-0">
                    <div class="w-11 h-11 rounded-full bg-green-100 flex items-center justify-center text-green-500">
                        <i class="ri-file-list-3-line text-xl"></i>
                    </div>
                </div>
                <div class="w-full pl-3">
                    <div class="text-gray-500 text-sm mb-1.5"><span class="font-semibold text-gray-900">Project Update</span> Your task "Design Homepage" has been completed</div>
                    <div class="text-xs text-blue-600">1 hour ago</div>
                </div>
            </a>
            <a href="#" class="flex px-4 py-3 hover:bg-gray-100">
                <div class="flex-shrink-0">
                    <div class="w-11 h-11 rounded-full bg-amber-100 flex items-center justify-center text-amber-500">
                        <i class="ri-calendar-event-line text-xl"></i>
                    </div>
                </div>
                <div class="w-full pl-3">
                    <div class="text-gray-500 text-sm mb-1.5"><span class="font-semibold text-gray-900">Calendar Reminder</span> Team meeting starts in 30 minutes in Room 301</div>
                    <div class="text-xs text-blue-600">3 hours ago</div>
                </div>
            </a>
        </div>
        <a href="#" class="block py-2 text-sm font-medium text-center text-gray-900 bg-gray-50 rounded-b-lg hover:bg-gray-100">
            View all notifications
        </a>
    </div>
</div>
```

## JavaScript for Dropdown Functionality

```javascript
document.addEventListener('DOMContentLoaded', function() {
    // Toggle dropdown visibility
    document.querySelectorAll('[data-dropdown-toggle]').forEach(toggleButton => {
        toggleButton.addEventListener('click', function(e) {
            e.preventDefault();
            e.stopPropagation();
            
            const targetId = this.getAttribute('data-dropdown-toggle');
            const targetDropdown = document.getElementById(targetId);
            
            if (!targetDropdown) return;
            
            // Toggle this dropdown
            targetDropdown.classList.toggle('hidden');
            
            // Close all other dropdowns
            document.querySelectorAll('[data-dropdown]').forEach(dropdown => {
                if (dropdown.id !== targetId) {
                    dropdown.classList.add('hidden');
                }
            });
        });
    });
    
    // Close all dropdowns when clicking outside
    document.addEventListener('click', function(e) {
        if (!e.target.closest('[data-dropdown]') && !e.target.closest('[data-dropdown-toggle]')) {
            document.querySelectorAll('[data-dropdown]').forEach(dropdown => {
                dropdown.classList.add('hidden');
            });
        }
    });
    
    // Handle hover dropdowns
    document.querySelectorAll('[data-dropdown-hover]').forEach(hoverElement => {
        const targetId = hoverElement.getAttribute('data-dropdown-hover');
        const targetDropdown = document.getElementById(targetId);
        
        if (!targetDropdown) return;
        
        hoverElement.addEventListener('mouseenter', function() {
            targetDropdown.classList.remove('hidden');
        });
        
        hoverElement.addEventListener('mouseleave', function(e) {
            // Check if we're not hovering over the dropdown itself
            if (!e.relatedTarget || !e.relatedTarget.closest(`#${targetId}`)) {
                targetDropdown.classList.add('hidden');
            }
        });
        
        targetDropdown.addEventListener('mouseleave', function() {
            targetDropdown.classList.add('hidden');
        });
    });
});
```
