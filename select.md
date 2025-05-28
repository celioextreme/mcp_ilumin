# Select Examples with Tailwind CSS

## Example 1: Basic Select Components
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-list-check text-xl mr-2"></i> Example 1: Basic Select Components
    </h2>
    <div class="space-y-5">
        <!-- Default Select -->
        <div>
            <label for="default-select" class="block mb-2 text-sm font-medium text-gray-700">Default Select</label>
            <select id="default-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                <option selected>Choose an option</option>
                <option value="option1">Option 1</option>
                <option value="option2">Option 2</option>
                <option value="option3">Option 3</option>
                <option value="option4">Option 4</option>
            </select>
        </div>
        
        <!-- Disabled Select -->
        <div>
            <label for="disabled-select" class="block mb-2 text-sm font-medium text-gray-700">Disabled Select</label>
            <select id="disabled-select" disabled class="bg-gray-100 border border-gray-300 text-gray-500 text-sm rounded-lg block w-full p-2.5 cursor-not-allowed">
                <option selected>Select is disabled</option>
                <option value="option1">Option 1</option>
                <option value="option2">Option 2</option>
            </select>
        </div>
    </div>
</div>
```

## Example 2: Select with Icons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-menu-search-line text-xl mr-2"></i> Example 2: Select with Icons
    </h2>
    <div class="space-y-5">
        <!-- Select with Left Icon -->
        <div>
            <label for="country-select" class="block mb-2 text-sm font-medium text-gray-700">Select Country</label>
            <div class="relative">
                <div class="absolute inset-y-0 start-0 flex items-center pl-3 pointer-events-none">
                    <i class="ri-earth-line text-gray-500"></i>
                </div>
                <select id="country-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5">
                    <option selected>Choose a country</option>
                    <option value="us">United States</option>
                    <option value="ca">Canada</option>
                    <option value="fr">France</option>
                    <option value="de">Germany</option>
                    <option value="jp">Japan</option>
                </select>
            </div>
        </div>
        
        <!-- Select with Right Icon -->
        <div>
            <label for="currency-select" class="block mb-2 text-sm font-medium text-gray-700">Select Currency</label>
            <div class="relative">
                <select id="currency-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pr-10 p-2.5">
                    <option selected>Choose a currency</option>
                    <option value="usd">USD - US Dollar</option>
                    <option value="eur">EUR - Euro</option>
                    <option value="gbp">GBP - British Pound</option>
                    <option value="jpy">JPY - Japanese Yen</option>
                </select>
                <div class="absolute inset-y-0 end-0 flex items-center pr-3 pointer-events-none">
                    <i class="ri-money-dollar-circle-line text-gray-500"></i>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 3: Select Sizes and Variants
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-aspect-ratio-line text-xl mr-2"></i> Example 3: Select Sizes and Variants
    </h2>
    <div class="space-y-6">
        <!-- Different Sizes -->
        <div class="space-y-4">
            <h3 class="text-lg font-medium text-gray-800">Select Sizes</h3>
            
            <div>
                <label for="small-select" class="block mb-2 text-sm font-medium text-gray-700">Small Select</label>
                <select id="small-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-xs rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2">
                    <option selected>Choose an option</option>
                    <option value="option1">Option 1</option>
                    <option value="option2">Option 2</option>
                </select>
            </div>
            
            <div>
                <label for="default-size-select" class="block mb-2 text-sm font-medium text-gray-700">Default Select</label>
                <select id="default-size-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                    <option selected>Choose an option</option>
                    <option value="option1">Option 1</option>
                    <option value="option2">Option 2</option>
                </select>
            </div>
            
            <div>
                <label for="large-select" class="block mb-2 text-sm font-medium text-gray-700">Large Select</label>
                <select id="large-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-base rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-3.5">
                    <option selected>Choose an option</option>
                    <option value="option1">Option 1</option>
                    <option value="option2">Option 2</option>
                </select>
            </div>
        </div>
    </div>
</div>
```

## Example 4: Multiple Select
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-checkbox-multiple-line text-xl mr-2"></i> Example 4: Multiple Select
    </h2>
    <div class="space-y-6">
        <!-- Basic Multiple Select -->
        <div>
            <label for="multi-select" class="block mb-2 text-sm font-medium text-gray-700">Select multiple options</label>
            <select multiple id="multi-select" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" size="4">
                <option value="html">HTML</option>
                <option value="css">CSS</option>
                <option value="javascript">JavaScript</option>
                <option value="php">PHP</option>
                <option value="python">Python</option>
                <option value="ruby">Ruby</option>
            </select>
            <p class="mt-1 text-xs text-gray-500">Hold down the Ctrl (Windows) or Command (Mac) button to select multiple options.</p>
        </div>
    </div>
</div>
```

## Example 5: Select with Add-ons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-add-box-line text-xl mr-2"></i> Example 5: Select with Add-ons
    </h2>
    <div class="space-y-6">
        <!-- Select with Prefix -->
        <div>
            <label for="currency-addon" class="block mb-2 text-sm font-medium text-gray-700">Currency Converter</label>
            <div class="flex">
                <span class="inline-flex items-center px-3 text-sm text-gray-900 bg-gray-200 border border-e-0 border-gray-300 rounded-s-lg">
                    <i class="ri-money-dollar-circle-line"></i>
                </span>
                <select id="currency-addon" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-e-lg border-s-0 focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                    <option value="usd" selected>USD</option>
                    <option value="eur">EUR</option>
                    <option value="gbp">GBP</option>
                    <option value="jpy">JPY</option>
                </select>
            </div>
        </div>
        
        <!-- Select with Suffix Button -->
        <div>
            <label for="search-category" class="block mb-2 text-sm font-medium text-gray-700">Search Category</label>
            <div class="flex">
                <select id="search-category" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-s-lg border-e-0 focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                    <option value="all" selected>All Categories</option>
                    <option value="electronics">Electronics</option>
                    <option value="clothing">Clothing</option>
                    <option value="books">Books</option>
                </select>
                <button type="button" class="inline-flex items-center px-4 text-sm font-medium text-white bg-blue-600 rounded-e-lg border border-blue-600 hover:bg-blue-700 focus:outline-none focus:ring-blue-300">
                    <i class="ri-search-line"></i>
                </button>
            </div>
        </div>
    </div>
</div>
```
