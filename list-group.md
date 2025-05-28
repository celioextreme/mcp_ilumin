# List Group Component Examples

## Example 1: Basic List Group
```html
<ul class="divide-y divide-gray-200 border border-gray-200 rounded-md overflow-hidden">
    <li class="p-4 bg-white hover:bg-gray-50">
        <span class="text-gray-700">Dashboard</span>
    </li>
    <li class="p-4 bg-white hover:bg-gray-50">
        <span class="text-gray-700">Settings</span>
    </li>
    <li class="p-4 bg-white hover:bg-gray-50">
        <span class="text-gray-700">Messages</span>
    </li>
    <li class="p-4 bg-white hover:bg-gray-50">
        <span class="text-gray-700">Profile</span>
    </li>
    <li class="p-4 bg-white hover:bg-gray-50">
        <span class="text-gray-700">Help Center</span>
    </li>
</ul>
```

## Example 2: List Group with Icons and Active State
```html
<ul class="divide-y divide-gray-200 border border-gray-200 rounded-md overflow-hidden">
    <li class="flex items-center p-4 bg-white hover:bg-gray-50">
        <i class="ri-home-line text-gray-500 mr-3"></i>
        <span class="text-gray-700">Home</span>
    </li>
    <li class="flex items-center p-4 bg-indigo-50 hover:bg-indigo-100 border-l-4 border-indigo-500">
        <i class="ri-dashboard-line text-indigo-500 mr-3"></i>
        <span class="font-medium text-indigo-700">Dashboard</span>
    </li>
    <li class="flex items-center p-4 bg-white hover:bg-gray-50">
        <i class="ri-settings-line text-gray-500 mr-3"></i>
        <span class="text-gray-700">Settings</span>
    </li>
    <li class="flex items-center p-4 bg-white hover:bg-gray-50">
        <i class="ri-message-2-line text-gray-500 mr-3"></i>
        <span class="text-gray-700">Messages</span>
        <span class="ml-auto bg-red-500 text-white text-xs px-2 py-0.5 rounded-full">3</span>
    </li>
</ul>
```

## Example 3: List Group with Actions
```html
<div class="border border-gray-200 rounded-md overflow-hidden">
    <div class="p-3 bg-gray-50 border-b border-gray-200">
        <h3 class="font-medium text-gray-700">Team Members</h3>
    </div>
    <ul class="divide-y divide-gray-200">
        <li class="p-4 bg-white hover:bg-gray-50 flex items-center justify-between">
            <div class="flex items-center">
                <div class="h-10 w-10 rounded-full bg-indigo-500 flex items-center justify-center text-white font-medium">JD</div>
                <div class="ml-3">
                    <p class="text-sm font-medium text-gray-800">Jane Doe</p>
                    <p class="text-xs text-gray-500">jane.doe@example.com</p>
                </div>
            </div>
            <div class="flex items-center space-x-2">
                <button class="text-gray-400 hover:text-blue-500">
                    <i class="ri-edit-line"></i>
                </button>
                <button class="text-gray-400 hover:text-red-500">
                    <i class="ri-delete-bin-line"></i>
                </button>
            </div>
        </li>
    </ul>
</div>
```

## Example 4: List Group with Complex Content
```html
<div class="border border-gray-200 rounded-lg overflow-hidden">
    <ul class="divide-y divide-gray-200">
        <li class="bg-white hover:bg-gray-50 p-4">
            <div class="flex justify-between">
                <h3 class="text-sm font-semibold text-gray-800">Project Status Update</h3>
                <span class="px-2 inline-flex text-xs leading-5 font-semibold rounded-full bg-green-100 text-green-800">Completed</span>
            </div>
            <div class="mt-2 text-sm text-gray-600">
                <p>All project milestones have been met for Q2. Ready for client presentation next week.</p>
            </div>
            <div class="mt-3 flex justify-between items-center">
                <p class="text-xs text-gray-500">Updated 3 hours ago</p>
                <div class="flex -space-x-2 overflow-hidden">
                    <img class="inline-block h-6 w-6 rounded-full ring-2 ring-white" src="https://randomuser.me/api/portraits/women/11.jpg" alt="">
                    <img class="inline-block h-6 w-6 rounded-full ring-2 ring-white" src="https://randomuser.me/api/portraits/men/13.jpg" alt="">
                </div>
            </div>
        </li>
    </ul>
</div>
```

## Example 5: Interactive List Group with Expandable Content
```html
<div class="border border-gray-200 rounded-lg overflow-hidden">
    <div class="accordion">
        <!-- Item 1 -->
        <div class="border-b border-gray-200">
            <button class="w-full flex items-center justify-between p-4 focus:outline-none hover:bg-gray-50 transition-colors" onclick="toggleAccordion('accordion-1')">
                <div class="flex items-center">
                    <i class="ri-file-list-line text-blue-500 mr-3"></i>
                    <span class="font-medium text-gray-800">Getting Started Guide</span>
                </div>
                <i class="ri-arrow-down-s-line text-gray-400 accordion-icon" id="icon-accordion-1"></i>
            </button>
            <div class="hidden p-4 pt-0 pl-11 bg-gray-50" id="accordion-1">
                <p class="text-sm text-gray-600">This guide will walk you through the setup process for your new account.</p>
                <div class="mt-3">
                    <a href="#" class="inline-flex items-center text-sm text-blue-600 hover:text-blue-800">
                        <i class="ri-download-line mr-1"></i> Download PDF
                    </a>
                </div>
            </div>
        </div>
    </div>
</div>

<script>
    function toggleAccordion(id) {
        const content = document.getElementById(id);
        const icon = document.getElementById(`icon-${id}`);
        
        if (content.classList.contains('hidden')) {
            content.classList.remove('hidden');
            icon.classList.add('transform', 'rotate-180');
        } else {
            content.classList.add('hidden');
            icon.classList.remove('transform', 'rotate-180');
        }
    }
</script>
```
