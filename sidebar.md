# Sidebar Examples with Tailwind CSS

## Example 1: Basic Left Sidebar
```html
<!-- Sidebar -->
<div class="w-full md:w-64 bg-white border-r border-gray-200">
    <div class="flex items-center justify-center h-16 bg-blue-600">
        <span class="text-white text-xl font-semibold">Dashboard</span>
    </div>
    <nav class="p-4">
        <ul class="space-y-2">
            <li>
                <a href="#" class="flex items-center p-2 text-gray-700 bg-gray-100 rounded-lg">
                    <i class="ri-home-line mr-3 text-lg"></i>
                    <span>Home</span>
                </a>
            </li>
            <li>
                <a href="#" class="flex items-center p-2 text-gray-600 hover:bg-gray-100 rounded-lg transition-all">
                    <i class="ri-user-line mr-3 text-lg"></i>
                    <span>Profile</span>
                </a>
            </li>
            <li>
                <a href="#" class="flex items-center p-2 text-gray-600 hover:bg-gray-100 rounded-lg transition-all">
                    <i class="ri-notification-line mr-3 text-lg"></i>
                    <span>Notifications</span>
                    <span class="ml-auto bg-red-500 text-white text-xs font-medium px-2 py-0.5 rounded-full">5</span>
                </a>
            </li>
        </ul>
    </nav>
</div>
```

## Example 2: Collapsible Sidebar
```html
<!-- Sidebar -->
<div id="collapsibleSidebar" class="w-64 bg-gray-900 text-gray-200 fixed lg:relative inset-y-0 left-0 z-30 sidebar-transition sidebar-mobile lg:translate-x-0 h-full overflow-y-auto">
    <div class="p-4">
        <div class="flex items-center justify-between">
            <div class="flex items-center space-x-2">
                <div class="bg-blue-600 w-8 h-8 rounded-md flex items-center justify-center">
                    <i class="ri-dashboard-line text-xl"></i>
                </div>
                <span class="text-lg font-semibold">AdminPanel</span>
            </div>
            <button class="text-white p-1 lg:hidden" onclick="toggleSidebar()">
                <i class="ri-close-line text-xl"></i>
            </button>
        </div>
        
        <div class="mt-8">
            <div class="text-xs uppercase text-gray-400 font-semibold mb-4">Main</div>
            <nav>
                <a href="#" class="flex items-center px-4 py-3 text-white bg-blue-700 rounded-lg mb-1">
                    <i class="ri-home-line text-lg mr-3"></i>
                    <span>Dashboard</span>
                </a>
                <a href="#" class="flex items-center px-4 py-3 text-gray-300 hover:bg-gray-800 rounded-lg mb-1">
                    <i class="ri-bar-chart-line text-lg mr-3"></i>
                    <span>Analytics</span>
                </a>
            </nav>
        </div>
    </div>
</div>

<!-- JavaScript for toggle functionality -->
<script>
    function toggleSidebar() {
        const sidebar = document.getElementById('collapsibleSidebar');
        const overlay = document.getElementById('sidebarOverlay');
        
        sidebar.classList.toggle('open');
        
        if (overlay.classList.contains('hidden')) {
            overlay.classList.remove('hidden');
        } else {
            overlay.classList.add('hidden');
        }
    }
</script>

<!-- CSS for mobile sidebar -->
<style>
    .sidebar-transition {
        transition: all 0.3s ease-in-out;
    }
    
    @media (max-width: 768px) {
        .sidebar-mobile {
            transform: translateX(-100%);
        }
        
        .sidebar-mobile.open {
            transform: translateX(0);
        }
    }
</style>
```

## Example 3: Mini Sidebar with Hover
```html
<!-- Mini Sidebar -->
<div id="miniSidebar" class="sidebar-mini-width bg-gray-800 text-white flex flex-col relative group">
    <!-- Logo Area -->
    <div class="flex items-center justify-center h-16 bg-gray-900">
        <div class="text-xl font-bold px-3 flex items-center">
            <i class="ri-bar-chart-horizontal-line text-blue-500"></i>
            <span class="ml-3 opacity-0 group-hover:opacity-100 transition-opacity duration-300 absolute left-12 whitespace-nowrap">Analytics Pro</span>
        </div>
    </div>
    
    <!-- Navigation -->
    <nav class="flex-1 overflow-y-auto py-4">
        <ul>
            <li class="relative">
                <a href="#" class="flex items-center h-12 px-3 text-gray-300 hover:bg-gray-700 hover:text-white">
                    <i class="ri-dashboard-line text-xl"></i>
                    <span class="ml-3 opacity-0 group-hover:opacity-100 transition-opacity duration-300 absolute left-12 whitespace-nowrap">Dashboard</span>
                </a>
            </li>
            <li class="relative">
                <a href="#" class="flex items-center h-12 px-3 bg-blue-600 text-white">
                    <i class="ri-line-chart-line text-xl"></i>
                    <span class="ml-3 opacity-0 group-hover:opacity-100 transition-opacity duration-300 absolute left-12 whitespace-nowrap">Analytics</span>
                </a>
            </li>
        </ul>
    </nav>
</div>

<!-- CSS for mini sidebar -->
<style>
    .sidebar-mini-width {
        width: 5rem;
        transition: width 0.3s ease;
    }
    
    .content-with-mini-sidebar {
        margin-left: 5rem;
        transition: margin-left 0.3s ease;
    }
</style>
```

## Example 4: Multi-level Dropdown Sidebar
```html
<!-- Dropdown Sidebar -->
<nav class="p-4">
    <ul class="space-y-1">
        <li>
            <a href="#" class="flex items-center p-2 text-gray-700 bg-white rounded-lg shadow-sm">
                <i class="ri-home-line mr-3 text-blue-600"></i>
                <span>Dashboard</span>
            </a>
        </li>
        
        <!-- Dropdown Item -->
        <li class="dropdown">
            <button class="flex items-center justify-between w-full p-2 text-gray-600 hover:bg-white hover:text-gray-800 rounded-lg transition-colors" onclick="toggleDropdown('userDropdown')">
                <div class="flex items-center">
                    <i class="ri-user-line mr-3 text-gray-500"></i>
                    <span>User Management</span>
                </div>
                <i class="ri-arrow-down-s-line transition-transform" id="userDropdownIcon"></i>
            </button>
            <ul id="userDropdown" class="mt-1 ml-6 pl-3 border-l border-gray-200 hidden">
                <li>
                    <a href="#" class="flex items-center py-2 px-3 text-sm text-gray-600 hover:text-blue-600 transition-colors">
                        <i class="ri-user-add-line mr-2"></i>
                        <span>Add User</span>
                    </a>
                </li>
                <!-- More dropdown items -->
            </ul>
        </li>
        
        <!-- Nested Dropdown Item -->
        <li class="dropdown">
            <button class="flex items-center justify-between w-full p-2 text-gray-600 hover:bg-white hover:text-gray-800 rounded-lg transition-colors" onclick="toggleDropdown('contentDropdown')">
                <div class="flex items-center">
                    <i class="ri-file-list-line mr-3 text-gray-500"></i>
                    <span>Content</span>
                </div>
                <i class="ri-arrow-down-s-line transition-transform" id="contentDropdownIcon"></i>
            </button>
            <ul id="contentDropdown" class="mt-1 ml-6 pl-3 border-l border-gray-200 hidden">
                <li class="dropdown">
                    <button class="flex items-center justify-between w-full py-2 px-3 text-sm text-gray-600 hover:text-blue-600 transition-colors" onclick="toggleDropdown('categoriesDropdown')">
                        <div class="flex items-center">
                            <i class="ri-folders-line mr-2"></i>
                            <span>Categories</span>
                        </div>
                        <i class="ri-arrow-down-s-line transition-transform" id="categoriesDropdownIcon"></i>
                    </button>
                    <ul id="categoriesDropdown" class="mt-1 ml-4 pl-2 border-l border-gray-200 hidden">
                        <!-- Nested items -->
                    </ul>
                </li>
            </ul>
        </li>
    </ul>
</nav>

<!-- JavaScript for dropdown functionality -->
<script>
    function toggleDropdown(id) {
        const dropdown = document.getElementById(id);
        const icon = document.getElementById(id + 'Icon');
        
        if (dropdown.classList.contains('hidden')) {
            dropdown.classList.remove('hidden');
            icon.style.transform = 'rotate(180deg)';
        } else {
            dropdown.classList.add('hidden');
            icon.style.transform = 'rotate(0)';
        }
    }
</script>
```

## Example 5: Sidebar with Context Menu
```html
<!-- Sidebar with Context Menu -->
<div class="p-2">
    <div class="mb-4">
        <div class="flex items-center justify-between px-2 py-1.5 text-sm text-gray-600 font-medium">
            <span>PROJECTS</span>
            <i class="ri-arrow-down-s-line"></i>
        </div>
        <ul class="mt-1">
            <li>
                <a href="#" class="flex items-center p-2 text-gray-700 hover:bg-blue-50 hover:text-blue-700 rounded-md transition-colors" oncontextmenu="showContextMenu(event, 'projectContextMenu'); return false;">
                    <i class="ri-folder-line text-lg mr-3 text-amber-500"></i>
                    <span>Website Redesign</span>
                </a>
            </li>
            <!-- More items -->
        </ul>
    </div>
</div>

<!-- Context Menu -->
<div id="projectContextMenu" class="absolute shadow-lg border border-gray-200 bg-white rounded-md py-1 w-48 z-50 hidden menu-popover">
    <div class="px-3 py-2 text-xs font-semibold text-gray-500 border-b border-gray-100">PROJECT OPTIONS</div>
    <a href="#" class="flex items-center px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">
        <i class="ri-folder-open-line mr-2 text-amber-500"></i>
        <span>Open Project</span>
    </a>
    <a href="#" class="flex items-center px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">
        <i class="ri-share-line mr-2 text-gray-500"></i>
        <span>Share Project</span>
    </a>
    <!-- More context menu items -->
</div>

<!-- JavaScript for context menu -->
<script>
    function showContextMenu(event, menuId) {
        event.preventDefault();
        
        // Hide all context menus first
        hideContextMenus();
        
        const contextMenu = document.getElementById(menuId);
        contextMenu.style.top = `${event.pageY}px`;
        contextMenu.style.left = `${event.pageX}px`;
        contextMenu.classList.remove('hidden');
        
        // Adjust position if menu goes off screen
        const rect = contextMenu.getBoundingClientRect();
        const windowWidth = window.innerWidth;
        const windowHeight = window.innerHeight;
        
        if (rect.right > windowWidth) {
            contextMenu.style.left = `${event.pageX - rect.width}px`;
        }
        
        if (rect.bottom > windowHeight) {
            contextMenu.style.top = `${event.pageY - rect.height}px`;
        }
    }
    
    function hideContextMenus() {
        const menus = document.querySelectorAll('[id$="ContextMenu"]');
        menus.forEach(menu => {
            menu.classList.add('hidden');
        });
    }
    
    // Global click handler to hide context menus
    document.addEventListener('click', hideContextMenus);
</script>
```
