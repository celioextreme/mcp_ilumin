# Radio Button Examples with Tailwind CSS

## Example 1: Basic Radio Buttons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-radio-button-line text-xl mr-2"></i> Example 1: Basic Radio Buttons
    </h2>
    <div class="space-y-4">
        <p class="text-gray-700 mb-4">Select your preferred contact method:</p>
        
        <!-- Default Radio Button -->
        <div class="flex items-center">
            <input id="email-radio" type="radio" name="contact-method" value="email" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
            <label for="email-radio" class="ms-2 text-sm font-medium text-gray-900">Email</label>
        </div>
        
        <!-- Checked Radio Button -->
        <div class="flex items-center">
            <input checked id="phone-radio" type="radio" name="contact-method" value="phone" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
            <label for="phone-radio" class="ms-2 text-sm font-medium text-gray-900">Phone</label>
        </div>
        
        <!-- Disabled Radio Button -->
        <div class="flex items-center">
            <input disabled id="mail-radio" type="radio" name="contact-method" value="mail" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2 cursor-not-allowed opacity-50">
            <label for="mail-radio" class="ms-2 text-sm font-medium text-gray-400 cursor-not-allowed">Physical mail (unavailable)</label>
        </div>
    </div>
</div>
```

## Example 2: Styled Radio Buttons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-contrast-2-line text-xl mr-2"></i> Example 2: Styled Radio Buttons
    </h2>
    <div class="space-y-4">
        <p class="text-gray-700 mb-4">Select your priority level:</p>
        
        <!-- Green Radio Button -->
        <div class="flex items-center">
            <input id="low-radio" type="radio" name="priority" value="low" class="w-4 h-4 text-green-500 bg-gray-100 border-gray-300 focus:ring-green-500 focus:ring-2">
            <label for="low-radio" class="ms-2 text-sm font-medium text-gray-900">Low priority</label>
        </div>
        
        <!-- Orange Radio Button -->
        <div class="flex items-center">
            <input id="medium-radio" type="radio" name="priority" value="medium" class="w-4 h-4 text-orange-500 bg-gray-100 border-gray-300 focus:ring-orange-500 focus:ring-2">
            <label for="medium-radio" class="ms-2 text-sm font-medium text-gray-900">Medium priority</label>
        </div>
        
        <!-- Red Radio Button -->
        <div class="flex items-center">
            <input id="high-radio" type="radio" name="priority" value="high" class="w-4 h-4 text-red-500 bg-gray-100 border-gray-300 focus:ring-red-500 focus:ring-2">
            <label for="high-radio" class="ms-2 text-sm font-medium text-gray-900">High priority</label>
        </div>
    </div>
</div>
```

## Example 3: Custom Radio Button Design
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-paint-brush-line text-xl mr-2"></i> Example 3: Custom Radio Button Design
    </h2>
    <div class="space-y-6">
        <p class="text-gray-700 mb-4">Select your experience level:</p>
        
        <!-- Custom Radio with Animation -->
        <div class="space-y-4">
            <label class="inline-flex items-center cursor-pointer">
                <input type="radio" name="experience" value="beginner" class="hidden peer">
                <div class="relative w-5 h-5 border-2 border-gray-300 rounded-full peer-checked:border-blue-600 transition-colors duration-200">
                    <div class="absolute inset-0 scale-0 m-1 rounded-full peer-checked:scale-100 bg-blue-600 transition-transform duration-200 origin-center"></div>
                </div>
                <span class="ms-2 text-sm font-medium text-gray-900">Beginner</span>
            </label>
            
            <label class="inline-flex items-center cursor-pointer">
                <input type="radio" name="experience" value="intermediate" class="hidden peer" checked>
                <div class="relative w-5 h-5 border-2 border-gray-300 rounded-full peer-checked:border-blue-600 transition-colors duration-200">
                    <div class="absolute inset-0 scale-0 m-1 rounded-full peer-checked:scale-100 bg-blue-600 transition-transform duration-200 origin-center"></div>
                </div>
                <span class="ms-2 text-sm font-medium text-gray-900">Intermediate</span>
            </label>
        </div>
        
        <!-- Custom Pill Radio Buttons -->
        <div class="pt-4">
            <p class="text-gray-700 mb-4">Select your subscription tier:</p>
            <div class="inline-flex rounded-md shadow-sm" role="group">
                <label class="cursor-pointer">
                    <input type="radio" name="subscription" value="basic" class="peer sr-only" checked>
                    <span class="px-4 py-2 text-sm font-medium bg-white border border-gray-200 rounded-l-lg peer-checked:bg-blue-600 peer-checked:text-white peer-checked:border-blue-600 hover:bg-gray-100 hover:text-blue-700">
                        Basic
                    </span>
                </label>
                <label class="cursor-pointer">
                    <input type="radio" name="subscription" value="standard" class="peer sr-only">
                    <span class="px-4 py-2 text-sm font-medium bg-white border-t border-b border-gray-200 peer-checked:bg-blue-600 peer-checked:text-white peer-checked:border-blue-600 hover:bg-gray-100 hover:text-blue-700">
                        Standard
                    </span>
                </label>
                <label class="cursor-pointer">
                    <input type="radio" name="subscription" value="premium" class="peer sr-only">
                    <span class="px-4 py-2 text-sm font-medium bg-white border border-gray-200 rounded-r-lg peer-checked:bg-blue-600 peer-checked:text-white peer-checked:border-blue-600 hover:bg-gray-100 hover:text-blue-700">
                        Premium
                    </span>
                </label>
            </div>
        </div>
    </div>
</div>
```

## Example 4: Radio Buttons with Descriptions
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-file-list-3-line text-xl mr-2"></i> Example 4: Radio Buttons with Descriptions
    </h2>
    
    <p class="text-gray-700 mb-4">Choose a pricing plan:</p>
    
    <div class="space-y-4">
        <div class="flex items-start">
            <div class="flex items-center h-5">
                <input id="starter-plan" type="radio" name="pricing-plan" value="starter" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2">
            </div>
            <div class="ms-3 text-sm">
                <label for="starter-plan" class="font-medium text-gray-800">Starter Plan - $9/month</label>
                <p class="text-gray-500">Basic features for up to 3 users, 5GB storage, email support</p>
            </div>
        </div>
        
        <div class="flex items-start">
            <div class="flex items-center h-5">
                <input id="pro-plan" type="radio" name="pricing-plan" value="pro" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 focus:ring-2" checked>
            </div>
            <div class="ms-3 text-sm">
                <label for="pro-plan" class="font-medium text-gray-800">Professional Plan - $29/month</label>
                <p class="text-gray-500">Advanced features for up to 10 users, 20GB storage, priority support</p>
                <span class="inline-flex items-center mt-1 text-xs font-medium text-blue-600">
                    <i class="ri-check-line mr-1"></i>
                    Most Popular
                </span>
            </div>
        </div>
    </div>
</div>
```

## Example 5: Card Radio Buttons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-layout-cards-line text-xl mr-2"></i> Example 5: Card Radio Buttons
    </h2>
    
    <p class="text-gray-700 mb-4">Select your shipping method:</p>
    
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <!-- Standard Shipping Card -->
        <label class="cursor-pointer">
            <input type="radio" name="shipping" value="standard" class="peer hidden" checked>
            <div class="p-4 border-2 rounded-lg border-gray-200 peer-checked:border-blue-500 peer-checked:bg-blue-50 transition-colors duration-200">
                <div class="flex justify-between items-center mb-2">
                    <h3 class="font-medium text-gray-900">Standard Shipping</h3>
                    <div class="w-5 h-5 rounded-full border-2 flex items-center justify-center border-gray-300 peer-checked:border-blue-500 transition-colors duration-200">
                        <div class="w-2.5 h-2.5 rounded-full bg-blue-500 hidden peer-checked:block"></div>
                    </div>
                </div>
                <p class="text-sm text-gray-500">Delivery in 3-5 business days</p>
                <p class="text-base font-semibold text-gray-900 mt-2">Free</p>
            </div>
        </label>
    </div>
</div>
```
