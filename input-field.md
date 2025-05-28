# Input Field Examples with Tailwind CSS

## Example 1: Basic Input Fields
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-input-method-line text-xl mr-2"></i> Example 1: Basic Input Fields
    </h2>
    <div class="space-y-4">
        <!-- Default Input -->
        <div>
            <label for="default-input" class="block mb-2 text-sm font-medium text-gray-700">Default Input</label>
            <input type="text" id="default-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="Enter your text here">
        </div>
        
        <!-- Disabled Input -->
        <div>
            <label for="disabled-input" class="block mb-2 text-sm font-medium text-gray-700">Disabled Input</label>
            <input type="text" id="disabled-input" class="bg-gray-100 border border-gray-300 text-gray-500 text-sm rounded-lg block w-full p-2.5 cursor-not-allowed" placeholder="Disabled input" disabled>
        </div>
        
        <!-- Success Input -->
        <div>
            <label for="success-input" class="block mb-2 text-sm font-medium text-gray-700">Success Input</label>
            <input type="text" id="success-input" class="bg-green-50 border border-green-500 text-green-900 text-sm rounded-lg focus:ring-green-500 focus:border-green-500 block w-full p-2.5" placeholder="Success input">
            <p class="mt-1 text-sm text-green-600">
                <i class="ri-check-line inline"></i> This input value is valid!
            </p>
        </div>
        
        <!-- Error Input -->
        <div>
            <label for="error-input" class="block mb-2 text-sm font-medium text-gray-700">Error Input</label>
            <input type="text" id="error-input" class="bg-red-50 border border-red-500 text-red-900 text-sm rounded-lg focus:ring-red-500 focus:border-red-500 block w-full p-2.5" placeholder="Error input">
            <p class="mt-1 text-sm text-red-600">
                <i class="ri-error-warning-line inline"></i> This field is required!
            </p>
        </div>
    </div>
</div>
```

## Example 2: Input with Icons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-input-cursor-move text-xl mr-2"></i> Example 2: Input with Icons
    </h2>
    <div class="space-y-6">
        <!-- Left Icon Input -->
        <div>
            <label for="email-input" class="block mb-2 text-sm font-medium text-gray-700">Email Address</label>
            <div class="relative">
                <div class="absolute inset-y-0 start-0 flex items-center pl-3 pointer-events-none">
                    <i class="ri-mail-line text-gray-500"></i>
                </div>
                <input type="email" id="email-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" placeholder="name@example.com">
            </div>
        </div>
        
        <!-- Right Icon Input -->
        <div>
            <label for="search-input" class="block mb-2 text-sm font-medium text-gray-700">Search</label>
            <div class="relative">
                <input type="text" id="search-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pr-10 p-2.5" placeholder="Search...">
                <div class="absolute inset-y-0 end-0 flex items-center pr-3">
                    <i class="ri-search-line text-gray-500"></i>
                </div>
            </div>
        </div>
        
        <!-- Password with Toggle Visibility -->
        <div>
            <label for="password-input" class="block mb-2 text-sm font-medium text-gray-700">Password</label>
            <div class="relative">
                <input type="password" id="password-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pr-10 p-2.5" placeholder="••••••••">
                <div class="absolute inset-y-0 end-0 flex items-center pr-3">
                    <button type="button" class="text-gray-500 hover:text-gray-700 focus:outline-none" onclick="togglePasswordVisibility()">
                        <i id="password-icon" class="ri-eye-off-line"></i>
                    </button>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 3: Input Sizes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-ruler-line text-xl mr-2"></i> Example 3: Input Sizes
    </h2>
    <div class="space-y-4">
        <!-- Small Input -->
        <div>
            <label for="small-input" class="block mb-2 text-sm font-medium text-gray-700">Small Input</label>
            <input type="text" id="small-input" class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-xs focus:ring-blue-500 focus:border-blue-500" placeholder="Small size input">
        </div>
        
        <!-- Default Input -->
        <div>
            <label for="default-size-input" class="block mb-2 text-sm font-medium text-gray-700">Default Input</label>
            <input type="text" id="default-size-input" class="block w-full p-2.5 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-sm focus:ring-blue-500 focus:border-blue-500" placeholder="Default size input">
        </div>
        
        <!-- Large Input -->
        <div>
            <label for="large-input" class="block mb-2 text-sm font-medium text-gray-700">Large Input</label>
            <input type="text" id="large-input" class="block w-full p-4 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 text-base focus:ring-blue-500 focus:border-blue-500" placeholder="Large size input">
        </div>
    </div>
</div>
```

## Example 4: Input with Labels and Helpers
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-information-line text-xl mr-2"></i> Example 4: Input with Labels and Helpers
    </h2>
    <div class="space-y-6">
        <!-- Floating Label Input -->
        <div class="relative">
            <input type="text" id="floating-input" class="block px-2.5 pb-2.5 pt-4 w-full text-sm text-gray-900 bg-transparent rounded-lg border border-gray-300 appearance-none focus:outline-none focus:ring-0 focus:border-blue-600 peer" placeholder=" " />
            <label for="floating-input" class="absolute text-sm text-gray-500 duration-300 transform -translate-y-4 scale-75 top-2 z-10 origin-[0] bg-white px-2 peer-focus:px-2 peer-focus:text-blue-600 peer-placeholder-shown:scale-100 peer-placeholder-shown:-translate-y-1/2 peer-placeholder-shown:top-1/2 peer-focus:top-2 peer-focus:scale-75 peer-focus:-translate-y-4 start-1">Floating Label</label>
        </div>
        
        <!-- Input with Helper Text -->
        <div>
            <label for="helper-input" class="block mb-2 text-sm font-medium text-gray-700">Username</label>
            <input type="text" id="helper-input" aria-describedby="helper-text-explanation" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="username">
            <p id="helper-text-explanation" class="mt-2 text-sm text-gray-500">
                <i class="ri-information-line inline-block"></i> Your username must be 8-20 characters long and contain only letters and numbers.
            </p>
        </div>
    </div>
</div>
```

## Example 5: Input Groups
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-group-line text-xl mr-2"></i> Example 5: Input Groups
    </h2>
    <div class="space-y-6">
        <!-- Input with Prefix -->
        <div>
            <label for="price-input" class="block mb-2 text-sm font-medium text-gray-700">Price</label>
            <div class="flex">
                <span class="inline-flex items-center px-3 text-sm text-gray-900 bg-gray-200 border border-r-0 border-gray-300 rounded-l-md">
                    $
                </span>
                <input type="number" id="price-input" class="rounded-none rounded-r-lg bg-gray-50 border border-gray-300 text-gray-900 focus:ring-blue-500 focus:border-blue-500 block flex-1 min-w-0 w-full text-sm p-2.5" placeholder="0.00">
            </div>
        </div>
        
        <!-- Input with Suffix -->
        <div>
            <label for="weight-input" class="block mb-2 text-sm font-medium text-gray-700">Weight</label>
            <div class="flex">
                <input type="number" id="weight-input" class="rounded-none rounded-l-lg bg-gray-50 border border-gray-300 text-gray-900 focus:ring-blue-500 focus:border-blue-500 block flex-1 min-w-0 w-full text-sm p-2.5" placeholder="0">
                <span class="inline-flex items-center px-3 text-sm text-gray-900 bg-gray-200 border border-l-0 border-gray-300 rounded-r-md">
                    kg
                </span>
            </div>
        </div>
        
        <!-- Input with Button -->
        <div>
            <label for="search-button-input" class="block mb-2 text-sm font-medium text-gray-700">Search</label>
            <div class="flex">
                <input type="search" id="search-button-input" class="rounded-none rounded-l-lg bg-gray-50 border border-gray-300 text-gray-900 focus:ring-blue-500 focus:border-blue-500 block flex-1 min-w-0 w-full text-sm p-2.5" placeholder="Search...">
                <button type="button" class="inline-flex items-center px-4 text-sm font-medium text-white bg-blue-600 rounded-r-lg border border-blue-600 hover:bg-blue-700 focus:outline-none focus:ring-blue-300">
                    <i class="ri-search-line mr-2"></i>
                    Search
                </button>
            </div>
        </div>
    </div>
</div>
```
