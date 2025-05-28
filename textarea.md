# Textarea Examples with Tailwind CSS

## Example 1: Basic Textarea Components
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-text-wrap text-xl mr-2"></i> Example 1: Basic Textarea Components
    </h2>
    <div class="space-y-6">
        <!-- Default Textarea -->
        <div>
            <label for="default-textarea" class="block mb-2 text-sm font-medium text-gray-700">Default Textarea</label>
            <textarea id="default-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Write your thoughts here..."></textarea>
        </div>

        <!-- Disabled Textarea -->
        <div>
            <label for="disabled-textarea" class="block mb-2 text-sm font-medium text-gray-700">Disabled Textarea</label>
            <textarea id="disabled-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-500 bg-gray-100 rounded-lg border border-gray-300 cursor-not-allowed" disabled placeholder="This textarea is disabled" aria-label="disabled textarea"></textarea>
        </div>

        <!-- Helper Text Textarea -->
        <div>
            <label for="helper-textarea" class="block mb-2 text-sm font-medium text-gray-700">Your message</label>
            <textarea id="helper-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Leave a comment..."></textarea>
            <p class="mt-2 text-xs text-gray-500">
                <i class="ri-information-line inline-flex"></i> Your comment will be visible to other users.
            </p>
        </div>
    </div>
</div>
```

## Example 2: Textarea Validation States
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-checkbox-circle-line text-xl mr-2"></i> Example 2: Textarea Validation States
    </h2>
    <div class="space-y-6">
        <!-- Success State -->
        <div>
            <label for="success-textarea" class="block mb-2 text-sm font-medium text-gray-700">Success state</label>
            <textarea id="success-textarea" rows="4" class="block p-2.5 w-full text-sm text-green-900 bg-green-50 rounded-lg border border-green-500 focus:ring-green-500 focus:border-green-500" placeholder="This is a success state..."></textarea>
            <p class="mt-2 text-sm text-green-600 dark:text-green-500">
                <i class="ri-check-line mr-1"></i> Your message has been validated successfully!
            </p>
        </div>

        <!-- Error State -->
        <div>
            <label for="error-textarea" class="block mb-2 text-sm font-medium text-gray-700">Error state</label>
            <textarea id="error-textarea" rows="4" class="block p-2.5 w-full text-sm text-red-900 bg-red-50 rounded-lg border border-red-500 focus:ring-red-500 focus:border-red-500" placeholder="This is an error state..."></textarea>
            <p class="mt-2 text-sm text-red-600">
                <i class="ri-error-warning-line mr-1"></i> Please enter at least 20 characters.
            </p>
        </div>
    </div>
</div>
```

## Example 3: Textarea Sizes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-fullscreen-line text-xl mr-2"></i> Example 3: Textarea Sizes
    </h2>
    <div class="space-y-6">
        <!-- Small Size -->
        <div>
            <label for="small-textarea" class="block mb-2 text-sm font-medium text-gray-700">Small textarea</label>
            <textarea id="small-textarea" rows="2" class="block p-2 w-full text-xs text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Small textarea..."></textarea>
        </div>

        <!-- Default Size -->
        <div>
            <label for="default-size-textarea" class="block mb-2 text-sm font-medium text-gray-700">Default textarea</label>
            <textarea id="default-size-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Default size textarea..."></textarea>
        </div>

        <!-- Large Size -->
        <div>
            <label for="large-textarea" class="block mb-2 text-sm font-medium text-gray-700">Large textarea</label>
            <textarea id="large-textarea" rows="6" class="block p-3 w-full text-base text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Large textarea..."></textarea>
        </div>
    </div>
</div>
```

## Example 4: Styled Textareas
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-paint-brush-line text-xl mr-2"></i> Example 4: Styled Textareas
    </h2>
    <div class="space-y-6">
        <!-- Rounded Textarea -->
        <div>
            <label for="rounded-textarea" class="block mb-2 text-sm font-medium text-gray-700">Rounded textarea</label>
            <textarea id="rounded-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-3xl border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Rounded corners..."></textarea>
        </div>

        <!-- Custom Border Color -->
        <div>
            <label for="purple-textarea" class="block mb-2 text-sm font-medium text-purple-700">Purple bordered textarea</label>
            <textarea id="purple-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-purple-50 rounded-lg border-2 border-purple-400 focus:ring-purple-500 focus:border-purple-500" placeholder="Purple theme..."></textarea>
        </div>

        <!-- Underlined Style -->
        <div>
            <label for="underline-textarea" class="block mb-2 text-sm font-medium text-gray-700">Underlined textarea</label>
            <textarea id="underline-textarea" rows="4" class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none focus:outline-none focus:ring-0 focus:border-blue-600" placeholder="Underlined style..."></textarea>
        </div>
    </div>
</div>
```

## Example 5: Textarea with Addons
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-add-circle-line text-xl mr-2"></i> Example 5: Textarea with Addons
    </h2>
    <div class="space-y-6">
        <!-- Textarea with Character Counter -->
        <div>
            <label for="counter-textarea" class="block mb-2 text-sm font-medium text-gray-700">Character counter</label>
            <textarea id="counter-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Type your message here..." maxlength="200"></textarea>
            <div class="flex justify-between mt-2">
                <p class="text-xs text-gray-500">Maximum 200 characters</p>
                <p class="text-xs text-gray-500"><span id="current">0</span>/200</p>
            </div>
        </div>

        <!-- Textarea with Icon -->
        <div>
            <label for="icon-textarea" class="block mb-2 text-sm font-medium text-gray-700">Textarea with icon</label>
            <div class="relative">
                <div class="absolute top-3 left-3 flex items-center pointer-events-none">
                    <i class="ri-message-2-line text-gray-500"></i>
                </div>
                <textarea id="icon-textarea" rows="4" class="block p-2.5 pl-10 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Start typing..."></textarea>
            </div>
        </div>

        <!-- Textarea with Button -->
        <div>
            <label for="button-textarea" class="block mb-2 text-sm font-medium text-gray-700">Comment form</label>
            <textarea id="button-textarea" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-t-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Write a comment..."></textarea>
            <div class="flex items-center justify-between px-3 py-2 border border-t-0 border-gray-300 bg-gray-50 rounded-b-lg">
                <div class="flex space-x-1">
                    <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
                        <i class="ri-emotion-line"></i>
                    </button>
                    <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
                        <i class="ri-image-line"></i>
                    </button>
                    <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
                        <i class="ri-link"></i>
                    </button>
                </div>
                <button type="button" class="inline-flex items-center py-2 px-4 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:ring-blue-300">
                    <i class="ri-send-plane-line mr-1"></i> Post comment
                </button>
            </div>
        </div>
    </div>
</div>
```
