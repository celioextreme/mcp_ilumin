# File Input Examples with Tailwind CSS and Remix Icons

## Example 1: Basic File Input
```html
<div class="mb-5">
    <label class="block mb-2 text-sm font-medium text-gray-900" for="basic-file-input">Upload file</label>
    <input class="block w-full text-sm text-gray-900 border border-gray-300 rounded-lg cursor-pointer bg-gray-50 focus:outline-none" id="basic-file-input" type="file">
</div>
```

## Example 2: File Input with Help Text
```html
<div class="mb-5">
    <label class="block mb-2 text-sm font-medium text-gray-900" for="help-text-file">Upload file</label>
    <input class="block w-full text-sm text-gray-900 border border-gray-300 rounded-lg cursor-pointer bg-gray-50 focus:outline-none" aria-describedby="file_input_help" id="help-text-file" type="file">
    <p class="mt-1 text-sm text-gray-500" id="file_input_help">SVG, PNG, JPG or GIF (MAX. 2MB).</p>
</div>
```

## Example 3: Styled File Input with Button
```html
<div class="flex items-center justify-center w-full">
    <label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 hover:bg-gray-100">
        <div class="flex flex-col items-center justify-center pt-5 pb-6">
            <i class="ri-upload-cloud-2-line text-4xl text-gray-500 mb-3"></i>
            <p class="mb-2 text-sm text-gray-500"><span class="font-semibold">Click to upload</span> or drag and drop</p>
            <p class="text-xs text-gray-500">SVG, PNG, JPG or GIF (MAX. 2MB)</p>
        </div>
        <input id="dropzone-file" type="file" class="hidden" />
    </label>
</div>
```

## Example 4: Multiple File Upload
```html
<div class="mb-5">
    <label class="block mb-2 text-sm font-medium text-gray-900" for="multiple-files">Upload multiple files</label>
    <input class="block w-full text-sm text-gray-900 border border-gray-300 rounded-lg cursor-pointer bg-gray-50 focus:outline-none" id="multiple-files" type="file" multiple>
</div>

<div class="mt-4">
    <h3 class="text-sm font-medium text-gray-900 mb-3">Selected files:</h3>
    <ul class="max-w-md divide-y divide-gray-200">
        <li class="pb-3 sm:pb-4">
            <div class="flex items-center space-x-4 rtl:space-x-reverse">
                <div class="flex-shrink-0">
                    <i class="ri-file-image-line text-xl text-blue-600"></i>
                </div>
                <div class="flex-1 min-w-0">
                    <p class="text-sm font-medium text-gray-900 truncate">
                        profile-picture.jpg
                    </p>
                    <p class="text-sm text-gray-500 truncate">
                        756 KB
                    </p>
                </div>
                <div class="inline-flex items-center text-base font-semibold text-gray-900">
                    <button type="button" class="text-red-600 hover:text-red-800">
                        <i class="ri-delete-bin-line"></i>
                    </button>
                </div>
            </div>
        </li>
        <li class="py-3 sm:py-4">
            <div class="flex items-center space-x-4 rtl:space-x-reverse">
                <div class="flex-shrink-0">
                    <i class="ri-file-text-line text-xl text-green-600"></i>
                </div>
                <div class="flex-1 min-w-0">
                    <p class="text-sm font-medium text-gray-900 truncate">
                        resume.pdf
                    </p>
                    <p class="text-sm text-gray-500 truncate">
                        1.2 MB
                    </p>
                </div>
                <div class="inline-flex items-center text-base font-semibold text-gray-900">
                    <button type="button" class="text-red-600 hover:text-red-800">
                        <i class="ri-delete-bin-line"></i>
                    </button>
                </div>
            </div>
        </li>
    </ul>
</div>
```

## Example 5: File Upload with Progress and Preview
```html
<div class="mb-5">
    <label class="block mb-2 text-sm font-medium text-gray-900" for="preview-file">Upload profile image</label>
    <input class="block w-full text-sm text-gray-900 border border-gray-300 rounded-lg cursor-pointer bg-gray-50 focus:outline-none" id="preview-file" type="file" accept="image/*">
</div>

<div class="mt-4 grid grid-cols-1 md:grid-cols-2 gap-4">
    <div>
        <p class="text-sm font-medium text-gray-900 mb-2">Upload progress:</p>
        <div class="w-full bg-gray-200 rounded-full h-2.5">
            <div class="bg-blue-600 h-2.5 rounded-full" style="width: 75%"></div>
        </div>
        <div class="flex justify-between mt-1">
            <span class="text-xs text-gray-500">75%</span>
            <span class="text-xs text-gray-500">768 KB / 1024 KB</span>
        </div>
    </div>
    
    <div>
        <p class="text-sm font-medium text-gray-900 mb-2">Image preview:</p>
        <div class="relative">
            <img class="h-auto max-w-full rounded-lg border border-gray-200" src="https://via.placeholder.com/150" alt="Image preview">
            <button type="button" class="absolute top-2 right-2 text-gray-400 bg-white rounded-lg p-1.5 hover:bg-gray-200 hover:text-gray-900 focus:outline-none">
                <i class="ri-close-line text-lg"></i>
            </button>
        </div>
    </div>
</div>

<div class="mt-4 flex justify-end">
    <button type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center">
        <i class="ri-upload-2-line mr-2"></i>
        Upload Image
    </button>
</div>
```
