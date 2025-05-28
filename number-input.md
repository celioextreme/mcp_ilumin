# Number Input Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Number Input
```html
<div class="mb-5">
    <label for="number-input" class="block mb-2 text-sm font-medium text-gray-900">Choose a number:</label>
    <div class="relative">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
            <i class="ri-hashtag text-gray-500"></i>
        </div>
        <input type="number" id="number-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" placeholder="Enter a number" required>
    </div>
</div>
```

## Example 2: Number Input with Min/Max and Step
```html
<div class="mb-5">
    <label for="number-input-constraints" class="block mb-2 text-sm font-medium text-gray-900">Rating (1-5, step 0.5):</label>
    <div class="relative">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
            <i class="ri-star-line text-gray-500"></i>
        </div>
        <input type="number" id="number-input-constraints" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" min="1" max="5" step="0.5" value="3" required>
    </div>
    <p class="mt-2 text-sm text-gray-500">Min: 1, Max: 5, Step: 0.5</p>
</div>
```

## Example 3: Number Input with Increment/Decrement Buttons
```html
<div class="mb-5">
    <label for="quantity-input" class="block mb-2 text-sm font-medium text-gray-900">Product quantity:</label>
    <div class="relative flex items-center max-w-[8rem]">
        <button type="button" id="decrement-button" class="bg-gray-100 hover:bg-gray-200 border border-gray-300 rounded-s-lg p-3 h-11 focus:ring-gray-100 focus:ring-2 focus:outline-none">
            <i class="ri-subtract-line text-gray-900"></i>
        </button>
        <input type="number" id="quantity-input" class="bg-gray-50 border-x-0 border-gray-300 h-11 text-gray-900 text-center text-sm focus:ring-blue-500 focus:border-blue-500 block w-full py-2.5" min="1" max="100" value="1" required>
        <button type="button" id="increment-button" class="bg-gray-100 hover:bg-gray-200 border border-gray-300 rounded-e-lg p-3 h-11 focus:ring-gray-100 focus:ring-2 focus:outline-none">
            <i class="ri-add-line text-gray-900"></i>
        </button>
    </div>
</div>

<script>
    // Script for increment/decrement buttons
    document.addEventListener('DOMContentLoaded', function() {
        const decrementButton = document.getElementById('decrement-button');
        const incrementButton = document.getElementById('increment-button');
        const quantityInput = document.getElementById('quantity-input');
        
        decrementButton.addEventListener('click', () => {
            const currentValue = parseInt(quantityInput.value);
            if (currentValue > parseInt(quantityInput.min)) {
                quantityInput.value = currentValue - 1;
            }
        });
        
        incrementButton.addEventListener('click', () => {
            const currentValue = parseInt(quantityInput.value);
            if (currentValue < parseInt(quantityInput.max)) {
                quantityInput.value = currentValue + 1;
            }
        });
    });
</script>
```

## Example 4: Number Input with Currency
```html
<div class="mb-5">
    <label for="price-input" class="block mb-2 text-sm font-medium text-gray-900">Price (USD):</label>
    <div class="relative">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
            <i class="ri-currency-dollar text-gray-500"></i>
        </div>
        <input type="number" id="price-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" min="0" step="0.01" placeholder="0.00" required>
    </div>
</div>

<div class="mb-5">
    <label for="price-input-euro" class="block mb-2 text-sm font-medium text-gray-900">Price (EUR):</label>
    <div class="flex">
        <span class="inline-flex items-center px-3 text-sm text-gray-900 bg-gray-200 border border-e-0 border-gray-300 rounded-s-md">
            <i class="ri-currency-euro text-gray-500"></i>
        </span>
        <input type="number" id="price-input-euro" class="rounded-none rounded-e-lg bg-gray-50 border border-gray-300 text-gray-900 focus:ring-blue-500 focus:border-blue-500 block flex-1 min-w-0 w-full text-sm p-2.5" min="0" step="0.01" placeholder="0.00" required>
    </div>
</div>
```

## Example 5: Number Input with Validation and Styling
```html
<div class="grid md:grid-cols-2 gap-6">
    <div>
        <label for="valid-number" class="block mb-2 text-sm font-medium text-green-700">Valid number</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-checkbox-circle-line text-green-600"></i>
            </div>
            <input type="number" id="valid-number" class="bg-green-50 border border-green-500 text-green-900 text-sm rounded-lg focus:ring-green-500 focus:border-green-500 block w-full ps-10 p-2.5" value="42" required>
            <div class="absolute inset-y-0 end-0 flex items-center pe-3 pointer-events-none">
                <i class="ri-check-line text-green-500"></i>
            </div>
        </div>
        <p class="mt-1 text-sm text-green-600">Valid input!</p>
    </div>
    
    <div>
        <label for="error-number" class="block mb-2 text-sm font-medium text-red-700">Age (18+)</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-error-warning-line text-red-500"></i>
            </div>
            <input type="number" id="error-number" class="bg-red-50 border border-red-500 text-red-900 text-sm rounded-lg focus:ring-red-500 focus:border-red-500 block w-full ps-10 p-2.5" value="16" min="18" required>
            <div class="absolute inset-y-0 end-0 flex items-center pe-3 pointer-events-none">
                <i class="ri-close-line text-red-500"></i>
            </div>
        </div>
        <p class="mt-1 text-sm text-red-600">Must be 18 years or older.</p>
    </div>
</div>
```
