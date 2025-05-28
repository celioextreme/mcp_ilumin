# Pagination Component Examples with Tailwind CSS and Remix Icons

## Example 1: Simple Pagination

```html
<nav aria-label="Page navigation">
    <ul class="flex items-center -space-x-px h-10 text-base">
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 ms-0 leading-tight text-gray-500 bg-white border border-e-0 border-gray-300 rounded-s-lg hover:bg-gray-100 hover:text-gray-700">
                <span class="sr-only">Previous</span>
                <i class="ri-arrow-left-s-line w-3.5 h-3.5"></i>
            </a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">1</a>
        </li>
        <li>
            <a href="#" aria-current="page" class="flex items-center justify-center px-4 h-10 text-blue-600 border border-gray-300 bg-blue-50 hover:bg-blue-100 hover:text-blue-700">2</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">3</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">4</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">5</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 rounded-e-lg hover:bg-gray-100 hover:text-gray-700">
                <span class="sr-only">Next</span>
                <i class="ri-arrow-right-s-line w-3.5 h-3.5"></i>
            </a>
        </li>
    </ul>
</nav>
```

## Example 2: Pagination with Icons

```html
<nav aria-label="Page navigation">
    <ul class="flex items-center -space-x-px h-10 text-base">
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 ms-0 leading-tight text-gray-500 bg-white border border-e-0 border-gray-300 rounded-s-lg hover:bg-gray-100 hover:text-gray-700">
                <span class="sr-only">First</span>
                <i class="ri-arrow-left-double-line"></i>
            </a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">
                <span class="sr-only">Previous</span>
                <i class="ri-arrow-left-s-line"></i>
            </a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">1</a>
        </li>
        <li>
            <a href="#" aria-current="page" class="flex items-center justify-center px-4 h-10 text-blue-600 border border-gray-300 bg-blue-50 hover:bg-blue-100 hover:text-blue-700">2</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">3</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">
                <span class="sr-only">Next</span>
                <i class="ri-arrow-right-s-line"></i>
            </a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-4 h-10 leading-tight text-gray-500 bg-white border border-gray-300 rounded-e-lg hover:bg-gray-100 hover:text-gray-700">
                <span class="sr-only">Last</span>
                <i class="ri-arrow-right-double-line"></i>
            </a>
        </li>
    </ul>
</nav>
```

## Example 3: Rounded Button Pagination

```html
<div class="flex flex-col items-center">
    <!-- Help text -->
    <span class="text-sm text-gray-700 mb-3">
        Showing <span class="font-semibold text-gray-900">1</span> to <span class="font-semibold text-gray-900">10</span> of <span class="font-semibold text-gray-900">100</span> Entries
    </span>
    <!-- Pagination -->
    <div class="inline-flex gap-1 mt-2">
        <a href="#" class="px-3 py-2 text-sm font-medium text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:ring-blue-300">
            <i class="ri-arrow-left-s-line"></i>
        </a>
        <a href="#" class="px-3 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-200">1</a>
        <a href="#" class="px-3 py-2 text-sm font-medium text-white bg-blue-700 border border-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:ring-blue-300">2</a>
        <a href="#" class="px-3 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-200">3</a>
        <a href="#" class="px-3 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-200">4</a>
        <a href="#" class="px-3 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-200">5</a>
        <a href="#" class="px-3 py-2 text-sm font-medium text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:ring-blue-300">
            <i class="ri-arrow-right-s-line"></i>
        </a>
    </div>
</div>
```

## Example 4: Pagination with Ellipsis

```html
<nav aria-label="Page navigation">
    <ul class="flex items-center -space-x-px h-8 text-sm">
        <li>
            <a href="#" class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 rounded-l-lg hover:bg-gray-100 hover:text-gray-700">Previous</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">1</a>
        </li>
        <li>
            <span class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">...</span>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">4</a>
        </li>
        <li>
            <a href="#" aria-current="page" class="flex items-center justify-center px-3 h-8 text-blue-600 border border-gray-300 bg-blue-50 hover:bg-blue-100 hover:text-blue-700">5</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">6</a>
        </li>
        <li>
            <span class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">...</span>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700">10</a>
        </li>
        <li>
            <a href="#" class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 rounded-r-lg hover:bg-gray-100 hover:text-gray-700">Next</a>
        </li>
    </ul>
</nav>
```

## Example 5: Pagination with Custom Styling

```html
<div class="flex justify-center">
    <div class="inline-flex items-center justify-center gap-3">
        <a href="#" class="inline-flex items-center justify-center w-10 h-10 bg-purple-600 rounded-full text-white shadow-md hover:bg-purple-700 focus:ring-4 focus:ring-purple-300 transition-all">
            <i class="ri-skip-back-line"></i>
        </a>
        <a href="#" class="inline-flex items-center justify-center w-10 h-10 bg-purple-600 rounded-full text-white shadow-md hover:bg-purple-700 focus:ring-4 focus:ring-purple-300 transition-all">
            <i class="ri-arrow-left-s-line"></i>
        </a>
        <span class="px-4 py-2 text-sm font-medium text-gray-700">Page 5 of 10</span>
        <a href="#" class="inline-flex items-center justify-center w-10 h-10 bg-purple-600 rounded-full text-white shadow-md hover:bg-purple-700 focus:ring-4 focus:ring-purple-300 transition-all">
            <i class="ri-arrow-right-s-line"></i>
        </a>
        <a href="#" class="inline-flex items-center justify-center w-10 h-10 bg-purple-600 rounded-full text-white shadow-md hover:bg-purple-700 focus:ring-4 focus:ring-purple-300 transition-all">
            <i class="ri-skip-forward-line"></i>
        </a>
    </div>
</div>

<!-- Jump to page form -->
<div class="flex justify-center mt-4">
    <form class="flex items-center space-x-2">
        <label for="page-number" class="text-sm text-gray-700">Jump to:</label>
        <input type="number" id="page-number" min="1" max="10" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-purple-500 focus:border-purple-500 w-16 p-2" placeholder="Page">
        <button type="submit" class="text-white bg-purple-600 hover:bg-purple-700 focus:ring-4 focus:outline-none focus:ring-purple-300 font-medium rounded-lg text-sm p-2">
            <i class="ri-arrow-right-line"></i>
        </button>
    </form>
</div>
```
