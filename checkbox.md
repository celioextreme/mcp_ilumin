# Checkbox Examples with Tailwind CSS

## Example 1: Basic Checkboxes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-checkbox-line text-xl mr-2"></i> Example 1: Basic Checkboxes
    </h2>
    <div class="space-y-4">
        <!-- Default Checkbox -->
        <div class="flex items-center">
            <input id="default-checkbox" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2">
            <label for="default-checkbox" class="ms-2 text-sm font-medium text-gray-900">Default checkbox</label>
        </div>
        
        <!-- Checked Checkbox -->
        <div class="flex items-center">
            <input checked id="checked-checkbox" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2">
            <label for="checked-checkbox" class="ms-2 text-sm font-medium text-gray-900">Checked checkbox</label>
        </div>
        
        <!-- Disabled Checkbox -->
        <div class="flex items-center">
            <input disabled id="disabled-checkbox" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2 cursor-not-allowed opacity-50">
            <label for="disabled-checkbox" class="ms-2 text-sm font-medium text-gray-400 cursor-not-allowed">Disabled checkbox</label>
        </div>
        
        <!-- Disabled Checked Checkbox -->
        <div class="flex items-center">
            <input disabled checked id="disabled-checked-checkbox" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2 cursor-not-allowed opacity-70">
            <label for="disabled-checked-checkbox" class="ms-2 text-sm font-medium text-gray-400 cursor-not-allowed">Disabled checked checkbox</label>
        </div>
    </div>
</div>
```

## Example 2: Styled Checkboxes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-checkbox-multiple-line text-xl mr-2"></i> Example 2: Styled Checkboxes
    </h2>
    <div class="space-y-4">
        <!-- Green Checkbox -->
        <div class="flex items-center">
            <input id="green-checkbox" type="checkbox" class="w-4 h-4 text-green-500 bg-gray-100 border-gray-300 rounded focus:ring-green-500 focus:ring-2">
            <label for="green-checkbox" class="ms-2 text-sm font-medium text-gray-900">Green checkbox</label>
        </div>
        
        <!-- Red Checkbox -->
        <div class="flex items-center">
            <input id="red-checkbox" type="checkbox" class="w-4 h-4 text-red-500 bg-gray-100 border-gray-300 rounded focus:ring-red-500 focus:ring-2">
            <label for="red-checkbox" class="ms-2 text-sm font-medium text-gray-900">Red checkbox</label>
        </div>
        
        <!-- Purple Checkbox -->
        <div class="flex items-center">
            <input id="purple-checkbox" type="checkbox" class="w-4 h-4 text-purple-500 bg-gray-100 border-gray-300 rounded focus:ring-purple-500 focus:ring-2">
            <label for="purple-checkbox" class="ms-2 text-sm font-medium text-gray-900">Purple checkbox</label>
        </div>
        
        <!-- Larger Checkbox -->
        <div class="flex items-center">
            <input id="large-checkbox" type="checkbox" class="w-6 h-6 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2">
            <label for="large-checkbox" class="ms-2 text-base font-medium text-gray-900">Larger checkbox</label>
        </div>
    </div>
</div>
```

## Example 3: Custom Checkbox Design
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-paint-brush-line text-xl mr-2"></i> Example 3: Custom Checkbox Design
    </h2>
    <div class="space-y-4">
        <!-- Custom Checkbox with Check Icon -->
        <label class="inline-flex items-center cursor-pointer">
            <input type="checkbox" class="hidden peer">
            <div class="relative w-5 h-5 border border-gray-300 rounded bg-gray-50 peer-checked:bg-blue-600 peer-checked:border-blue-600 transition-all duration-200">
                <svg class="absolute w-4 h-4 text-white scale-0 peer-checked:scale-100 transition-transform duration-200 top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2" fill="currentColor" viewBox="0 0 20 20">
                    <path d="M7.293 13.293a1 1 0 0 1-1.414 0l-2.5-2.5a1 1 0 0 1 1.414-1.414L6.5 11.086l5.293-5.293a1 1 0 0 1 1.414 1.414l-6 6z"/>
                </svg>
            </div>
            <span class="ms-2 text-sm font-medium text-gray-900">Custom checkbox with icon</span>
        </label>
        
        <!-- Custom Switch Style -->
        <label class="inline-flex items-center cursor-pointer">
            <input type="checkbox" class="sr-only peer">
            <div class="relative w-11 h-6 bg-gray-200 peer-focus:outline-none peer-focus:ring-4 peer-focus:ring-blue-300 rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-blue-600"></div>
            <span class="ms-3 text-sm font-medium text-gray-900">Switch style checkbox</span>
        </label>
    </div>
</div>
```

## Example 4: Grouped Checkboxes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-list-check text-xl mr-2"></i> Example 4: Grouped Checkboxes
    </h2>
    
    <!-- Notification Preferences Group -->
    <fieldset class="mb-6">
        <legend class="text-base font-semibold text-gray-800 mb-3">Notification Preferences</legend>
        <div class="space-y-3">
            <div class="flex items-start">
                <div class="flex items-center h-5">
                    <input id="email-notifications" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2">
                </div>
                <div class="ms-3 text-sm">
                    <label for="email-notifications" class="font-medium text-gray-800">Email notifications</label>
                    <p class="text-gray-500">Get notified via email about account activity</p>
                </div>
            </div>
            <div class="flex items-start">
                <div class="flex items-center h-5">
                    <input id="push-notifications" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 focus:ring-2" checked>
                </div>
                <div class="ms-3 text-sm">
                    <label for="push-notifications" class="font-medium text-gray-800">Push notifications</label>
                    <p class="text-gray-500">Get mobile push notifications about account activity</p>
                </div>
            </div>
        </div>
    </fieldset>
</div>
```

## Example 5: Card Checkboxes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-checkbox-multiple-blank-line text-xl mr-2"></i> Example 5: Card Checkboxes
    </h2>
    
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <!-- Card Checkbox 1 -->
        <label class="cursor-pointer">
            <input type="checkbox" class="peer hidden">
            <div class="p-4 border-2 rounded-lg border-gray-200 peer-checked:border-blue-500 peer-checked:bg-blue-50 transition-colors duration-200">
                <div class="flex justify-between items-start">
                    <div>
                        <i class="ri-flight-takeoff-line text-3xl text-blue-600 mb-2"></i>
                        <h3 class="font-medium text-gray-900">Air Travel</h3>
                    </div>
                    <div class="w-5 h-5 rounded-full border-2 flex items-center justify-center border-gray-300 peer-checked:border-blue-500 peer-checked:bg-blue-500 transition-colors duration-200">
                        <svg class="w-3 h-3 text-white hidden peer-checked:block" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"></path>
                        </svg>
                    </div>
                </div>
                <p class="text-sm text-gray-500 mt-1">Include airfare in your travel package</p>
            </div>
        </label>
    </div>
</div>
```
