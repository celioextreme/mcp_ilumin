# Phone Input Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Phone Input
```html
<div class="mb-5">
    <label for="phone-input" class="block mb-2 text-sm font-medium text-gray-900">Phone number</label>
    <div class="relative">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
            <i class="ri-phone-line text-gray-500"></i>
        </div>
        <input type="tel" id="phone-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" placeholder="123-456-7890" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" required>
    </div>
    <p class="mt-2 text-sm text-gray-500">Format: 123-456-7890</p>
</div>
```

## Example 2: Phone Input with Country Code
```html
<div class="mb-5">
    <label for="phone-input-country" class="block mb-2 text-sm font-medium text-gray-900">Phone number with country code</label>
    <div class="flex">
        <div class="inline-flex items-center px-3 text-sm text-gray-900 bg-gray-200 border border-e-0 border-gray-300 rounded-s-md">
            <span class="flex items-center">
                <i class="ri-global-line mr-1"></i>
                +1
            </span>
        </div>
        <div class="relative w-full">
            <input type="tel" id="phone-input-country" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-e-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="(555) 987-6543" required>
        </div>
    </div>
</div>
```

## Example 3: Phone Input with Country Selector
```html
<div class="mb-5">
    <label for="phone-input-full" class="block mb-2 text-sm font-medium text-gray-900">Phone number with country</label>
    <div class="flex">
        <button id="dropdown-phone-button" data-dropdown-toggle="dropdown-phone" class="flex-shrink-0 z-10 inline-flex items-center py-2.5 px-4 text-sm font-medium text-center text-gray-900 bg-gray-100 border border-gray-300 rounded-s-lg hover:bg-gray-200 focus:ring-4 focus:outline-none focus:ring-gray-100" type="button">
            <i class="ri-flag-line mr-2"></i> US +1 <i class="ri-arrow-down-s-line ms-2"></i>
        </button>
        <div class="relative w-full">
            <input type="text" id="phone-input-full" class="block p-2.5 w-full z-20 text-sm text-gray-900 bg-gray-50 rounded-e-lg border-s-0 border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="123 456 789" pattern="[0-9]{3} [0-9]{3} [0-9]{3}" required>
        </div>
    </div>
    <!-- Dropdown menu (would be functional with JavaScript) -->
    <div id="dropdown-phone" class="hidden z-10 w-full max-h-72 overflow-y-auto bg-white rounded-lg shadow">
        <ul class="py-2 text-sm text-gray-700" aria-labelledby="dropdown-phone-button">
            <li>
                <button type="button" class="inline-flex w-full px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">
                    <i class="ri-flag-line mr-2"></i> United States +1
                </button>
            </li>
            <li>
                <button type="button" class="inline-flex w-full px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">
                    <i class="ri-flag-line mr-2"></i> United Kingdom +44
                </button>
            </li>
            <!-- Additional countries would go here -->
        </ul>
    </div>
</div>
```

## Example 4: Phone Input with Validation
```html
<form>
    <div class="mb-3">
        <label for="phone-success" class="block mb-2 text-sm font-medium text-green-700">Valid phone number</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-phone-line text-green-600"></i>
            </div>
            <input type="tel" id="phone-success" class="bg-green-50 border border-green-500 text-green-900 text-sm rounded-lg focus:ring-green-500 focus:border-green-500 block w-full ps-10 p-2.5" placeholder="555-123-4567" value="555-123-4567" required>
            <div class="absolute inset-y-0 end-0 flex items-center pe-3 pointer-events-none">
                <i class="ri-check-line text-green-500"></i>
            </div>
        </div>
        <p class="mt-1 text-sm text-green-600">Valid format!</p>
    </div>
    
    <div>
        <label for="phone-error" class="block mb-2 text-sm font-medium text-red-700">Phone number</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-phone-line text-red-500"></i>
            </div>
            <input type="tel" id="phone-error" class="bg-red-50 border border-red-500 text-red-900 text-sm rounded-lg focus:ring-red-500 focus:border-red-500 block w-full ps-10 p-2.5" placeholder="123-456-7890" value="1234" required>
            <div class="absolute inset-y-0 end-0 flex items-center pe-3 pointer-events-none">
                <i class="ri-error-warning-line text-red-500"></i>
            </div>
        </div>
        <p class="mt-1 text-sm text-red-600">Please enter a valid phone number (format: 123-456-7890)</p>
    </div>
</form>
```

## Example 5: Phone Input with SMS Verification
```html
<div class="space-y-4">
    <div class="mb-2">
        <label for="phone-verify" class="block mb-2 text-sm font-medium text-gray-900">Phone number for verification</label>
        <div class="flex">
            <div class="relative w-full">
                <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                    <i class="ri-smartphone-line text-gray-500"></i>
                </div>
                <input type="tel" id="phone-verify" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" placeholder="Enter your phone number" required>
            </div>
            <button type="button" class="ml-2 px-4 py-2 bg-blue-600 text-white font-medium text-sm rounded-lg hover:bg-blue-700 focus:outline-none focus:ring-4 focus:ring-blue-300">
                Verify
            </button>
        </div>
    </div>
    
    <div class="mb-5">
        <label for="verification-code" class="block mb-2 text-sm font-medium text-gray-900">Verification code</label>
        <div class="flex space-x-2">
            <input type="text" maxlength="1" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm text-center rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-10 h-12 p-0" required>
            <input type="text" maxlength="1" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm text-center rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-10 h-12 p-0" required>
            <input type="text" maxlength="1" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm text-center rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-10 h-12 p-0" required>
            <input type="text" maxlength="1" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm text-center rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-10 h-12 p-0" required>
            <input type="text" maxlength="1" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm text-center rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-10 h-12 p-0" required>
            <input type="text" maxlength="1" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm text-center rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-10 h-12 p-0" required>
        </div>
        <div class="flex justify-between mt-3">
            <p class="text-sm text-gray-500">Code sent to +1 *** *** 7890</p>
            <button type="button" class="text-sm text-blue-600 hover:underline">Resend code</button>
        </div>
    </div>
    
    <button type="submit" class="w-full px-5 py-2.5 bg-green-600 hover:bg-green-700 text-white font-medium rounded-lg text-sm focus:ring-4 focus:outline-none focus:ring-green-300">
        Confirm verification
    </button>
</div>
```
