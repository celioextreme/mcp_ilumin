# Typography Examples with Tailwind CSS

## Example 1: Headings
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-text-wrap text-xl mr-2"></i> Example 1: Headings
    </h2>
    <div class="space-y-4">
        <h1 class="text-5xl font-bold text-gray-900">Heading 1 (text-5xl)</h1>
        <h2 class="text-4xl font-bold text-gray-800">Heading 2 (text-4xl)</h2>
        <h3 class="text-3xl font-semibold text-gray-700">Heading 3 (text-3xl)</h3>
        <h4 class="text-2xl font-semibold text-gray-700">Heading 4 (text-2xl)</h4>
        <h5 class="text-xl font-medium text-gray-700">Heading 5 (text-xl)</h5>
        <h6 class="text-lg font-medium text-gray-700">Heading 6 (text-lg)</h6>
    </div>
</div>
```

## Example 2: Paragraphs and Text Styling
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-paragraph text-xl mr-2"></i> Example 2: Paragraphs and Text Styling
    </h2>
    <div class="space-y-4">
        <p class="text-base text-gray-700 leading-relaxed">
            This is a <span class="font-bold">regular paragraph</span> with default styling. It uses text-base, text-gray-700, and leading-relaxed classes for comfortable reading.
        </p>
        
        <p class="text-sm text-gray-600 leading-relaxed">
            This is a <span class="italic">smaller paragraph</span> with text-sm class. Good for less important information or notes.
        </p>
        
        <p class="text-lg text-gray-800 leading-relaxed">
            This is a <span class="underline">larger paragraph</span> with text-lg class. Great for important information or introductions.
        </p>
        
        <div class="space-y-2">
            <p class="font-light">This text uses font-light weight.</p>
            <p class="font-normal">This text uses font-normal weight.</p>
            <p class="font-medium">This text uses font-medium weight.</p>
            <p class="font-semibold">This text uses font-semibold weight.</p>
            <p class="font-bold">This text uses font-bold weight.</p>
            <p class="font-extrabold">This text uses font-extrabold weight.</p>
        </div>
    </div>
</div>
```

## Example 3: Blockquotes
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-double-quotes-l text-xl mr-2"></i> Example 3: Blockquotes
    </h2>
    <div class="space-y-8">
        <!-- Simple Blockquote -->
        <blockquote class="p-4 border-l-4 border-blue-500 bg-blue-50 text-gray-700 italic">
            <p class="mb-2">The greatest glory in living lies not in never falling, but in rising every time we fall.</p>
            <footer class="text-sm text-gray-600">— Nelson Mandela</footer>
        </blockquote>
        
        <!-- Styled Blockquote with Icon -->
        <blockquote class="relative p-6 rounded-lg bg-gray-50 border border-gray-200">
            <div class="absolute top-0 left-0 transform -translate-y-1/2 -translate-x-1/2 w-10 h-10 flex items-center justify-center bg-indigo-600 rounded-full">
                <i class="ri-double-quotes-l text-white text-xl"></i>
            </div>
            <p class="text-lg font-medium text-gray-800 leading-relaxed mb-3">
                The future belongs to those who believe in the beauty of their dreams.
            </p>
            <footer class="flex items-center">
                <div class="w-10 h-10 rounded-full bg-indigo-200 flex items-center justify-center mr-3">
                    <i class="ri-user-line text-indigo-600"></i>
                </div>
                <div>
                    <p class="font-semibold text-gray-900">Eleanor Roosevelt</p>
                    <p class="text-sm text-gray-600">Former First Lady of the United States</p>
                </div>
            </footer>
        </blockquote>
    </div>
</div>
```

## Example 4: Lists
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-list-check text-xl mr-2"></i> Example 4: Lists
    </h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Unordered List -->
        <div>
            <h3 class="text-lg font-medium mb-3 text-gray-800">Unordered List</h3>
            <ul class="list-disc pl-5 space-y-2 text-gray-700">
                <li>First item with a bullet point</li>
                <li>Second item
                    <ul class="list-circle pl-5 mt-2 space-y-1">
                        <li>Nested item one</li>
                        <li>Nested item two</li>
                    </ul>
                </li>
                <li>Third item with a longer text that might wrap to the next line to show how the indentation works</li>
                <li>Fourth item</li>
            </ul>
        </div>
        
        <!-- Ordered List -->
        <div>
            <h3 class="text-lg font-medium mb-3 text-gray-800">Ordered List</h3>
            <ol class="list-decimal pl-5 space-y-2 text-gray-700">
                <li>First numbered item</li>
                <li>Second numbered item
                    <ol class="list-[lower-alpha] pl-5 mt-2 space-y-1">
                        <li>Nested item with letter a</li>
                        <li>Nested item with letter b</li>
                    </ol>
                </li>
                <li>Third numbered item</li>
                <li>Fourth numbered item</li>
            </ol>
        </div>
        
        <!-- Custom Icon List -->
        <div class="col-span-1 md:col-span-2 mt-4">
            <h3 class="text-lg font-medium mb-3 text-gray-800">Custom Icon List</h3>
            <ul class="space-y-3">
                <li class="flex items-start">
                    <i class="ri-check-line text-green-500 mt-1 mr-2"></i>
                    <span>Feature one with a custom checkmark icon</span>
                </li>
                <li class="flex items-start">
                    <i class="ri-check-line text-green-500 mt-1 mr-2"></i>
                    <span>Feature two with the same icon but can have a longer description to show how text wraps</span>
                </li>
                <li class="flex items-start">
                    <i class="ri-star-fill text-yellow-500 mt-1 mr-2"></i>
                    <span>Highlighted feature with a star icon</span>
                </li>
                <li class="flex items-start">
                    <i class="ri-close-line text-red-500 mt-1 mr-2"></i>
                    <span>Something not included, with a negative icon</span>
                </li>
            </ul>
        </div>
    </div>
</div>
```

## Example 5: Links and Text Decorations
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-links-line text-xl mr-2"></i> Example 5: Links and Text Decorations
    </h2>
    <div class="space-y-6">
        <!-- Standard Links -->
        <div class="space-y-2">
            <h3 class="text-lg font-medium text-gray-800">Standard Links</h3>
            <p class="text-gray-700">
                This is a paragraph with a <a href="#" class="text-blue-600 hover:text-blue-800 hover:underline">simple link</a> that changes color on hover.
            </p>
            <p class="text-gray-700">
                This is a paragraph with a <a href="#" class="text-blue-600 underline hover:text-blue-800">permanently underlined link</a> for better visibility.
            </p>
        </div>
        
        <!-- Styled Links -->
        <div class="space-y-3">
            <h3 class="text-lg font-medium text-gray-800">Styled Links</h3>
            <div class="space-y-2">
                <a href="#" class="inline-flex items-center text-blue-600 hover:text-blue-800">
                    <span>Learn more about our services</span>
                    <i class="ri-arrow-right-line ml-1"></i>
                </a>
                
                <a href="#" class="inline-flex items-center text-green-600 hover:text-green-800">
                    <i class="ri-download-line mr-1"></i>
                    <span>Download our brochure</span>
                </a>
                
                <a href="#" class="inline-block px-4 py-2 bg-blue-600 text-white rounded hover:bg-blue-700 transition-colors">
                    Button-styled link
                </a>
            </div>
        </div>
        
        <!-- Text Decorations -->
        <div class="space-y-2">
            <h3 class="text-lg font-medium text-gray-800">Text Decorations</h3>
            <div class="space-y-2 text-gray-700">
                <p class="underline decoration-solid">Solid underline</p>
                <p class="underline decoration-double">Double underline</p>
                <p class="underline decoration-dotted">Dotted underline</p>
                <p class="underline decoration-dashed">Dashed underline</p>
                <p class="underline decoration-wavy">Wavy underline</p>
                <p class="line-through">Line-through text</p>
                <p class="overline">Overline text</p>
            </div>
        </div>
    </div>
</div>
```
