# Breadcrumb Component Examples

## Example 1: Basic Breadcrumb

```html
<nav class="flex" aria-label="Breadcrumb">
    <ol class="inline-flex items-center space-x-1 md:space-x-3">
        <li class="inline-flex items-center">
            <a href="#" class="inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600">
                <i class="ri-home-line mr-2"></i>
                Home
            </a>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <a href="#" class="ml-1 text-sm font-medium text-gray-700 hover:text-blue-600 md:ml-2">Projects</a>
            </div>
        </li>
        <li aria-current="page">
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <span class="ml-1 text-sm font-medium text-gray-500 md:ml-2">Flowbite</span>
            </div>
        </li>
    </ol>
</nav>
```

## Example 2: Breadcrumb with Slash Dividers

```html
<nav class="flex" aria-label="Breadcrumb">
    <ol class="inline-flex items-center space-x-1 md:space-x-2">
        <li class="inline-flex items-center">
            <a href="#" class="inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600">
                <i class="ri-home-line mr-2"></i>
                Home
            </a>
        </li>
        <li>
            <div class="flex items-center">
                <span class="mx-1 text-gray-400">/</span>
                <a href="#" class="text-sm font-medium text-gray-700 hover:text-blue-600">Products</a>
            </div>
        </li>
        <li>
            <div class="flex items-center">
                <span class="mx-1 text-gray-400">/</span>
                <a href="#" class="text-sm font-medium text-gray-700 hover:text-blue-600">Electronics</a>
            </div>
        </li>
        <li aria-current="page">
            <div class="flex items-center">
                <span class="mx-1 text-gray-400">/</span>
                <span class="text-sm font-medium text-gray-500">Smartphones</span>
            </div>
        </li>
    </ol>
</nav>
```

## Example 3: Breadcrumb with Background

```html
<nav class="flex" aria-label="Breadcrumb">
    <ol class="inline-flex items-center p-2 bg-gray-50 rounded-lg">
        <li class="inline-flex items-center">
            <a href="#" class="inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600">
                <i class="ri-home-line mr-2"></i>
                Home
            </a>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line mx-2 text-gray-400"></i>
                <a href="#" class="text-sm font-medium text-gray-700 hover:text-blue-600">Category</a>
            </div>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line mx-2 text-gray-400"></i>
                <a href="#" class="text-sm font-medium text-gray-700 hover:text-blue-600">Products</a>
            </div>
        </li>
        <li aria-current="page">
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line mx-2 text-gray-400"></i>
                <span class="text-sm font-medium text-gray-500 bg-blue-100 px-2 py-1 rounded">Product Name</span>
            </div>
        </li>
    </ol>
</nav>
```

## Example 4: Breadcrumb with Icons

```html
<nav class="flex" aria-label="Breadcrumb">
    <ol class="inline-flex items-center space-x-1 md:space-x-3">
        <li class="inline-flex items-center">
            <a href="#" class="inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600">
                <i class="ri-home-line mr-2"></i>
                Home
            </a>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <a href="#" class="ml-1 inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600 md:ml-2">
                    <i class="ri-folder-line mr-1"></i>
                    Documents
                </a>
            </div>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <a href="#" class="ml-1 inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600 md:ml-2">
                    <i class="ri-file-list-line mr-1"></i>
                    Templates
                </a>
            </div>
        </li>
        <li aria-current="page">
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <span class="ml-1 inline-flex items-center text-sm font-medium text-gray-500 md:ml-2">
                    <i class="ri-file-line mr-1"></i>
                    Invoice.doc
                </span>
            </div>
        </li>
    </ol>
</nav>
```

## Example 5: Responsive Breadcrumb with Dropdown

```html
<!-- For desktop -->
<nav class="hidden md:flex mb-4" aria-label="Breadcrumb">
    <ol class="inline-flex items-center space-x-1 md:space-x-3">
        <li class="inline-flex items-center">
            <a href="#" class="inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600">
                <i class="ri-home-line mr-2"></i>
                Home
            </a>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <a href="#" class="ml-1 text-sm font-medium text-gray-700 hover:text-blue-600 md:ml-2">Shop</a>
            </div>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <a href="#" class="ml-1 text-sm font-medium text-gray-700 hover:text-blue-600 md:ml-2">Electronics</a>
            </div>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <a href="#" class="ml-1 text-sm font-medium text-gray-700 hover:text-blue-600 md:ml-2">Computers</a>
            </div>
        </li>
        <li aria-current="page">
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <span class="ml-1 text-sm font-medium text-gray-500 md:ml-2">Laptops</span>
            </div>
        </li>
    </ol>
</nav>

<!-- For mobile -->
<nav class="flex md:hidden" aria-label="Breadcrumb">
    <ol class="inline-flex items-center space-x-1">
        <li class="inline-flex items-center">
            <a href="#" class="inline-flex items-center text-sm font-medium text-gray-700 hover:text-blue-600">
                <i class="ri-home-line mr-1"></i>
            </a>
        </li>
        <li>
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <span class="relative ml-1">
                    <button id="dropdownBreadcrumbButton" class="text-sm font-medium text-gray-700 hover:text-blue-600 inline-flex items-center" type="button">
                        ...
                        <i class="ri-arrow-down-s-line ml-1"></i>
                    </button>
                    <div class="hidden absolute top-6 left-0 z-10 w-44 bg-white rounded-lg shadow-md p-2">
                        <ul class="py-1 text-sm text-gray-700">
                            <li>
                                <a href="#" class="block px-4 py-2 hover:bg-gray-100 rounded-md">Shop</a>
                            </li>
                            <li>
                                <a href="#" class="block px-4 py-2 hover:bg-gray-100 rounded-md">Electronics</a>
                            </li>
                            <li>
                                <a href="#" class="block px-4 py-2 hover:bg-gray-100 rounded-md">Computers</a>
                            </li>
                        </ul>
                    </div>
                </span>
            </div>
        </li>
        <li aria-current="page">
            <div class="flex items-center">
                <i class="ri-arrow-right-s-line text-gray-400"></i>
                <span class="ml-1 text-sm font-medium text-gray-500">Laptops</span>
            </div>
        </li>
    </ol>
</nav>
```
