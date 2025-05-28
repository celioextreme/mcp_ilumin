# Tailwind CSS Lists Examples

## Example 1: Basic List Styling

```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <!-- Unordered List -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Unordered List</h3>
        
        <ul class="list-disc pl-5 space-y-2 text-gray-700">
            <li>First item in the list</li>
            <li>Second item in the list</li>
            <li>Third item with a longer description that might wrap to the next line</li>
            <li>Fourth item in the list</li>
            <li>Fifth item in the list</li>
        </ul>
        
        <h3 class="text-lg font-medium text-gray-700 mt-6 mb-2">Nested List</h3>
        
        <ul class="list-disc pl-5 space-y-2 text-gray-700">
            <li>Parent item one</li>
            <li>
                Parent item two
                <ul class="list-circle pl-5 space-y-1 mt-1 text-gray-600">
                    <li>Nested child item 1</li>
                    <li>Nested child item 2</li>
                    <li>
                        Nested child item 3
                        <ul class="list-square pl-5 space-y-1 mt-1 text-gray-500">
                            <li>Deep nested item</li>
                            <li>Another deep nested item</li>
                        </ul>
                    </li>
                </ul>
            </li>
            <li>Parent item three</li>
        </ul>
    </div>
    
    <!-- Ordered List -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-2">Ordered List</h3>
        
        <ol class="list-decimal pl-5 space-y-2 text-gray-700">
            <li>First step in the process</li>
            <li>Second step in the process</li>
            <li>Third step with a longer description that might wrap to the next line</li>
            <li>Fourth step in the process</li>
            <li>Final step in the process</li>
        </ol>
    </div>
</div>
```

## Example 2: Custom Icon Lists

```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    <!-- Checkmark list -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-3">Feature List with Checkmarks</h3>
        
        <ul class="space-y-3">
            <li class="flex items-start">
                <i class="ri-checkbox-circle-fill text-green-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Responsive design ensures your site looks great on any device</span>
            </li>
            <li class="flex items-start">
                <i class="ri-checkbox-circle-fill text-green-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Lightning-fast performance with optimized code</span>
            </li>
            <li class="flex items-start">
                <i class="ri-checkbox-circle-fill text-green-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">SEO-friendly structure to improve search engine rankings</span>
            </li>
            <li class="flex items-start">
                <i class="ri-checkbox-circle-fill text-green-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">User-friendly interface with intuitive navigation</span>
            </li>
            <li class="flex items-start">
                <i class="ri-checkbox-circle-fill text-green-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Regular updates and dedicated support</span>
            </li>
        </ul>
    </div>
    
    <!-- Pros and cons list -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-3">Pros and Cons List</h3>
        
        <h4 class="font-medium text-gray-700 mb-2 flex items-center">
            <i class="ri-thumb-up-line text-blue-600 mr-2"></i>
            Pros
        </h4>
        <ul class="space-y-2 mb-4">
            <li class="flex items-start">
                <i class="ri-arrow-right-circle-fill text-blue-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Easy to learn and implement</span>
            </li>
            <li class="flex items-start">
                <i class="ri-arrow-right-circle-fill text-blue-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Highly customizable for any project</span>
            </li>
            <li class="flex items-start">
                <i class="ri-arrow-right-circle-fill text-blue-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Great community support</span>
            </li>
        </ul>
        
        <h4 class="font-medium text-gray-700 mb-2 flex items-center">
            <i class="ri-thumb-down-line text-red-600 mr-2"></i>
            Cons
        </h4>
        <ul class="space-y-2">
            <li class="flex items-start">
                <i class="ri-close-circle-fill text-red-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Can lead to large HTML files</span>
            </li>
            <li class="flex items-start">
                <i class="ri-close-circle-fill text-red-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Requires good organization for larger projects</span>
            </li>
            <li class="flex items-start">
                <i class="ri-close-circle-fill text-red-500 mt-1 mr-2 flex-shrink-0"></i>
                <span class="text-gray-700">Initial learning curve for utility-first approach</span>
            </li>
        </ul>
    </div>
</div>
```

## Example 3: Interactive Lists

```html
<div class="space-y-8">
    <!-- Clickable list with hover effects -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-3">Clickable List with Hover Effects</h3>
        
        <ul class="divide-y divide-gray-200 rounded-lg overflow-hidden border border-gray-200">
            <li class="group cursor-pointer">
                <a href="#" class="flex items-center p-4 hover:bg-gray-50 transition-colors">
                    <div class="flex-shrink-0 w-10 h-10 rounded-full bg-blue-100 flex items-center justify-center text-blue-600 group-hover:bg-blue-600 group-hover:text-white transition-colors">
                        <i class="ri-user-line"></i>
                    </div>
                    <div class="ml-4">
                        <h4 class="text-base font-medium text-gray-900 group-hover:text-blue-600">Account Settings</h4>
                        <p class="text-sm text-gray-500">Update your profile and preferences</p>
                    </div>
                    <div class="ml-auto">
                        <i class="ri-arrow-right-s-line text-gray-400 group-hover:text-blue-600 group-hover:transform group-hover:translate-x-1 transition-all"></i>
                    </div>
                </a>
            </li>
            <li class="group cursor-pointer">
                <a href="#" class="flex items-center p-4 hover:bg-gray-50 transition-colors">
                    <div class="flex-shrink-0 w-10 h-10 rounded-full bg-green-100 flex items-center justify-center text-green-600 group-hover:bg-green-600 group-hover:text-white transition-colors">
                        <i class="ri-shield-check-line"></i>
                    </div>
                    <div class="ml-4">
                        <h4 class="text-base font-medium text-gray-900 group-hover:text-green-600">Security</h4>
                        <p class="text-sm text-gray-500">Manage your password and 2FA settings</p>
                    </div>
                    <div class="ml-auto">
                        <i class="ri-arrow-right-s-line text-gray-400 group-hover:text-green-600 group-hover:transform group-hover:translate-x-1 transition-all"></i>
                    </div>
                </a>
            </li>
            <li class="group cursor-pointer">
                <a href="#" class="flex items-center p-4 hover:bg-gray-50 transition-colors">
                    <div class="flex-shrink-0 w-10 h-10 rounded-full bg-purple-100 flex items-center justify-center text-purple-600 group-hover:bg-purple-600 group-hover:text-white transition-colors">
                        <i class="ri-notification-line"></i>
                    </div>
                    <div class="ml-4">
                        <h4 class="text-base font-medium text-gray-900 group-hover:text-purple-600">Notifications</h4>
                        <p class="text-sm text-gray-500">Choose what alerts and notifications to receive</p>
                    </div>
                    <div class="ml-auto">
                        <i class="ri-arrow-right-s-line text-gray-400 group-hover:text-purple-600 group-hover:transform group-hover:translate-x-1 transition-all"></i>
                    </div>
                </a>
            </li>
        </ul>
    </div>
</div>
```

## Example 4: Complex List Components

```html
<div class="space-y-8">
    <!-- User list -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-3">User List</h3>
        
        <ul class="divide-y divide-gray-200 rounded-lg overflow-hidden border border-gray-200">
            <li class="p-4 hover:bg-gray-50">
                <div class="flex items-center justify-between">
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="User Avatar" class="w-10 h-10 rounded-full">
                        <div class="ml-3">
                            <h4 class="text-base font-medium text-gray-900">John Smith</h4>
                            <p class="text-sm text-gray-500">john.smith@example.com</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-2">
                        <span class="px-2 py-1 text-xs font-medium bg-green-100 text-green-800 rounded-full">Admin</span>
                        <button class="p-1 text-gray-400 hover:text-gray-600 focus:outline-none">
                            <i class="ri-more-2-fill"></i>
                        </button>
                    </div>
                </div>
            </li>
            <li class="p-4 hover:bg-gray-50">
                <div class="flex items-center justify-between">
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="User Avatar" class="w-10 h-10 rounded-full">
                        <div class="ml-3">
                            <h4 class="text-base font-medium text-gray-900">Sarah Johnson</h4>
                            <p class="text-sm text-gray-500">sarah.j@example.com</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-2">
                        <span class="px-2 py-1 text-xs font-medium bg-blue-100 text-blue-800 rounded-full">Editor</span>
                        <button class="p-1 text-gray-400 hover:text-gray-600 focus:outline-none">
                            <i class="ri-more-2-fill"></i>
                        </button>
                    </div>
                </div>
            </li>
        </ul>
    </div>
</div>
```

## Example 5: Animated and Interactive Lists

```html
<div class="space-y-8">
    <!-- Animated list items -->
    <div>
        <h3 class="text-lg font-medium text-gray-700 mb-3">Animated List Items</h3>
        
        <ul class="space-y-3" id="animated-list">
            <li class="transform transition-all duration-300 hover:-translate-y-1 hover:shadow-md">
                <div class="p-4 border border-gray-200 rounded-lg flex items-center">
                    <div class="flex-shrink-0 w-10 h-10 rounded-full bg-gradient-to-r from-blue-500 to-indigo-600 flex items-center justify-center text-white">
                        <i class="ri-home-line"></i>
                    </div>
                    <div class="ml-4">
                        <h4 class="text-base font-medium text-gray-900">Dashboard</h4>
                        <p class="text-sm text-gray-500">Overview of key metrics</p>
                    </div>
                    <div class="ml-auto">
                        <button class="text-gray-400 hover:text-gray-600">
                            <i class="ri-arrow-right-line"></i>
                        </button>
                    </div>
                </div>
            </li>
            <li class="transform transition-all duration-300 hover:-translate-y-1 hover:shadow-md">
                <div class="p-4 border border-gray-200 rounded-lg flex items-center">
                    <div class="flex-shrink-0 w-10 h-10 rounded-full bg-gradient-to-r from-green-500 to-emerald-600 flex items-center justify-center text-white">
                        <i class="ri-user-line"></i>
                    </div>
                    <div class="ml-4">
                        <h4 class="text-base font-medium text-gray-900">Profile</h4>
                        <p class="text-sm text-gray-500">Personal account settings</p>
                    </div>
                    <div class="ml-auto">
                        <button class="text-gray-400 hover:text-gray-600">
                            <i class="ri-arrow-right-line"></i>
                        </button>
                    </div>
                </div>
            </li>
            <li class="transform transition-all duration-300 hover:-translate-y-1 hover:shadow-md">
                <div class="p-4 border border-gray-200 rounded-lg flex items-center">
                    <div class="flex-shrink-0 w-10 h-10 rounded-full bg-gradient-to-r from-purple-500 to-pink-600 flex items-center justify-center text-white">
                        <i class="ri-settings-3-line"></i>
                    </div>
                    <div class="ml-4">
                        <h4 class="text-base font-medium text-gray-900">Settings</h4>
                        <p class="text-sm text-gray-500">App preferences and configuration</p>
                    </div>
                    <div class="ml-auto">
                        <button class="text-gray-400 hover:text-gray-600">
                            <i class="ri-arrow-right-line"></i>
                        </button>
                    </div>
                </div>
            </li>
        </ul>
    </div>
</div>
```
