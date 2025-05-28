# Tailwind CSS Links Examples

## Example 1: Basic Link Styles

```html
<div class="bg-white p-8 rounded-lg shadow-md mb-10">
    <h2 class="text-xl font-semibold text-gray-800 mb-4">Basic Link Styles</h2>
    
    <div class="space-y-6">
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Default Link</h3>
            <p class="text-gray-600 mb-2">A simple link with default underline on hover:</p>
            <a href="#" class="text-blue-600 hover:underline">Default link style</a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Permanent Underline</h3>
            <p class="text-gray-600 mb-2">A link that's always underlined:</p>
            <a href="#" class="text-indigo-600 underline hover:text-indigo-800">Always underlined link</a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Custom Underline</h3>
            <p class="text-gray-600 mb-2">A link with custom underline styling:</p>
            <a href="#" class="text-purple-600 decoration-2 decoration-purple-400 underline underline-offset-4 hover:decoration-purple-600">Custom underlined link</a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Dotted Underline</h3>
            <p class="text-gray-600 mb-2">A link with dotted underline that becomes solid on hover:</p>
            <a href="#" class="text-teal-600 underline decoration-dotted hover:decoration-solid">Dotted underline link</a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Wavy Underline</h3>
            <p class="text-gray-600 mb-2">A link with wavy underline:</p>
            <a href="#" class="text-pink-600 underline decoration-wavy decoration-2 underline-offset-2">Wavy underline link</a>
        </div>
    </div>
</div>
```

## Example 2: Animated Link Effects

```html
<div class="bg-white p-8 rounded-lg shadow-md mb-10">
    <h2 class="text-xl font-semibold text-gray-800 mb-4">Animated Link Effects</h2>
    
    <div class="space-y-8">
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Growing Underline</h3>
            <p class="text-gray-600 mb-2">A link with an underline that grows from the left:</p>
            <a href="#" class="relative text-blue-600 font-medium inline-block">
                Growing underline
                <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-blue-600 transition-all duration-300 group-hover:w-full"></span>
            </a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Color Transition</h3>
            <p class="text-gray-600 mb-2">A link with smooth color transition:</p>
            <a href="#" class="text-gray-700 transition-colors duration-300 hover:text-emerald-600">Color transition link</a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Border Bottom Slide</h3>
            <p class="text-gray-600 mb-2">A link with a slide-in bottom border:</p>
            <div class="inline-block relative">
                <a href="#" class="text-indigo-600 relative inline-block group">
                    Border slide effect
                    <span class="absolute -bottom-1 left-0 w-0 h-0.5 bg-indigo-600 transition-all duration-300 group-hover:w-full"></span>
                </a>
            </div>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Text Size Effect</h3>
            <p class="text-gray-600 mb-2">A link that scales slightly on hover:</p>
            <a href="#" class="text-amber-600 inline-block transition-transform duration-200 hover:scale-105">Text size effect</a>
        </div>
        
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Background Fill Effect</h3>
            <p class="text-gray-600 mb-2">A link with a background color that fills on hover:</p>
            <a href="#" class="relative px-2 py-1 font-medium text-purple-600 group">
                <span class="absolute inset-0 w-full h-full transition duration-300 ease-out transform -translate-x-2 -translate-y-1 bg-purple-100 group-hover:translate-x-0 group-hover:translate-y-0"></span>
                <span class="absolute inset-0 w-full h-full border-2 border-purple-600"></span>
                <span class="relative">Background fill</span>
            </a>
        </div>
    </div>
</div>
```

## Example 3: Links with Icons

```html
<div class="bg-white p-8 rounded-lg shadow-md mb-10">
    <h2 class="text-xl font-semibold text-gray-800 mb-4">Links with Icons</h2>
    
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="space-y-4">
            <h3 class="text-lg font-medium text-gray-700">External Links</h3>
            
            <a href="#" class="flex items-center gap-1 text-blue-600 hover:text-blue-800 group">
                <span>External link</span>
                <i class="ri-external-link-line transition-transform group-hover:translate-x-0.5 group-hover:-translate-y-0.5"></i>
            </a>
            
            <a href="#" class="flex items-center gap-1 text-blue-600 hover:text-blue-800">
                <i class="ri-arrow-right-up-line"></i>
                <span>Documentation link</span>
            </a>
            
            <a href="#" class="inline-flex items-center px-4 py-2 bg-gray-100 hover:bg-gray-200 text-gray-800 rounded-md transition-colors">
                <i class="ri-download-line mr-2"></i>
                <span>Download file</span>
            </a>
        </div>
        
        <div class="space-y-4">
            <h3 class="text-lg font-medium text-gray-700">Social Media Links</h3>
            
            <div class="flex space-x-4">
                <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors" aria-label="Twitter">
                    <i class="ri-twitter-x-line text-xl"></i>
                </a>
                <a href="#" class="text-gray-600 hover:text-blue-800 transition-colors" aria-label="Facebook">
                    <i class="ri-facebook-fill text-xl"></i>
                </a>
                <a href="#" class="text-gray-600 hover:text-pink-600 transition-colors" aria-label="Instagram">
                    <i class="ri-instagram-line text-xl"></i>
                </a>
                <a href="#" class="text-gray-600 hover:text-blue-500 transition-colors" aria-label="LinkedIn">
                    <i class="ri-linkedin-fill text-xl"></i>
                </a>
                <a href="#" class="text-gray-600 hover:text-red-600 transition-colors" aria-label="YouTube">
                    <i class="ri-youtube-fill text-xl"></i>
                </a>
            </div>
            
            <div class="pt-2 space-y-2">
                <a href="#" class="flex items-center gap-2 text-gray-700 hover:text-red-600 transition-colors group">
                    <i class="ri-youtube-fill text-xl group-hover:animate-pulse"></i>
                    <span>Watch our latest video</span>
                </a>
                
                <a href="#" class="flex items-center gap-2 text-gray-700 hover:text-blue-600 transition-colors group">
                    <i class="ri-twitter-x-line text-xl group-hover:rotate-6"></i>
                    <span>Follow us on Twitter</span>
                </a>
            </div>
        </div>
    </div>
</div>
```

## Example 4: Button-Style Links

```html
<div class="bg-white p-8 rounded-lg shadow-md mb-10">
    <h2 class="text-xl font-semibold text-gray-800 mb-4">Button-Style Links</h2>
    
    <div class="space-y-6">
        <div class="space-y-2">
            <h3 class="text-lg font-medium text-gray-700">Solid Buttons</h3>
            <div class="flex flex-wrap gap-3">
                <a href="#" class="inline-flex items-center px-4 py-2 bg-blue-600 text-white rounded-md hover:bg-blue-700 transition-colors duration-200">
                    Primary Button
                </a>
                <a href="#" class="inline-flex items-center px-4 py-2 bg-gray-800 text-white rounded-md hover:bg-gray-900 transition-colors duration-200">
                    Secondary Button
                </a>
                <a href="#" class="inline-flex items-center px-4 py-2 bg-green-600 text-white rounded-md hover:bg-green-700 transition-colors duration-200">
                    Success Button
                </a>
                <a href="#" class="inline-flex items-center px-4 py-2 bg-red-600 text-white rounded-md hover:bg-red-700 transition-colors duration-200">
                    Danger Button
                </a>
            </div>
        </div>
        
        <div class="space-y-2">
            <h3 class="text-lg font-medium text-gray-700">Outline Buttons</h3>
            <div class="flex flex-wrap gap-3">
                <a href="#" class="inline-flex items-center px-4 py-2 border border-blue-600 text-blue-600 rounded-md hover:bg-blue-50 transition-colors duration-200">
                    Primary Outline
                </a>
                <a href="#" class="inline-flex items-center px-4 py-2 border border-gray-800 text-gray-800 rounded-md hover:bg-gray-50 transition-colors duration-200">
                    Secondary Outline
                </a>
                <a href="#" class="inline-flex items-center px-4 py-2 border border-green-600 text-green-600 rounded-md hover:bg-green-50 transition-colors duration-200">
                    Success Outline
                </a>
                <a href="#" class="inline-flex items-center px-4 py-2 border border-red-600 text-red-600 rounded-md hover:bg-red-50 transition-colors duration-200">
                    Danger Outline
                </a>
            </div>
        </div>
    </div>
</div>
```

## Example 5: Link Groups and Advanced Styling

```html
<div class="bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold text-gray-800 mb-4">Link Groups and Advanced Styling</h2>
    
    <div class="space-y-6">
        <!-- Breadcrumb-Style Links -->
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Breadcrumb-Style Links</h3>
            <nav class="flex" aria-label="Breadcrumb">
                <ol class="inline-flex items-center space-x-1 md:space-x-2">
                    <li class="inline-flex items-center">
                        <a href="#" class="inline-flex items-center text-gray-700 hover:text-blue-600">
                            <i class="ri-home-line mr-2"></i>
                            Home
                        </a>
                    </li>
                    <li>
                        <div class="flex items-center">
                            <i class="ri-arrow-right-s-line text-gray-400 mx-1"></i>
                            <a href="#" class="text-gray-700 hover:text-blue-600">Products</a>
                        </div>
                    </li>
                    <li>
                        <div class="flex items-center">
                            <i class="ri-arrow-right-s-line text-gray-400 mx-1"></i>
                            <span class="text-gray-500">Current Item</span>
                        </div>
                    </li>
                </ol>
            </nav>
        </div>
        
        <!-- Tab-Style Links -->
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Tab-Style Links</h3>
            <div class="border-b border-gray-200">
                <nav class="-mb-px flex space-x-6">
                    <a href="#" class="border-b-2 border-blue-500 py-2 px-1 text-sm font-medium text-blue-600">
                        Active Tab
                    </a>
                    <a href="#" class="border-b-2 border-transparent py-2 px-1 text-sm font-medium text-gray-500 hover:text-gray-700 hover:border-gray-300">
                        Tab Link
                    </a>
                    <a href="#" class="border-b-2 border-transparent py-2 px-1 text-sm font-medium text-gray-500 hover:text-gray-700 hover:border-gray-300">
                        Another Tab
                    </a>
                    <a href="#" class="border-b-2 border-transparent py-2 px-1 text-sm font-medium text-gray-500 hover:text-gray-700 hover:border-gray-300">
                        Last Tab
                    </a>
                </nav>
            </div>
        </div>
        
        <!-- Gradient Link -->
        <div>
            <h3 class="text-lg font-medium text-gray-700 mb-2">Gradient Text Link</h3>
            <a href="#" class="inline-block text-transparent bg-clip-text bg-gradient-to-r from-pink-500 to-purple-600 font-bold hover:from-purple-600 hover:to-pink-500">
                Gradient Text Link
            </a>
        </div>
    </div>
</div>
```
