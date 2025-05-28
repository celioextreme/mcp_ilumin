# Chat Bubble Component Examples

## Example 1: Basic Chat Bubbles

```html
<div class="flex flex-col space-y-4">
    <!-- Received message -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=5" alt="User">
        </div>
        <div class="ml-3">
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm">
                <p class="text-sm text-gray-700">Hey! How are you doing today?</p>
            </div>
            <span class="text-xs text-gray-500 leading-none">10:15 AM</span>
        </div>
    </div>
    
    <!-- Sent message -->
    <div class="flex justify-end">
        <div class="mr-3">
            <div class="bg-blue-500 p-3 rounded-lg rounded-tr-none shadow-sm">
                <p class="text-sm text-white">Hi! I'm doing great, thanks for asking. How about you?</p>
            </div>
            <span class="text-xs text-gray-500 leading-none flex justify-end">10:16 AM</span>
        </div>
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=8" alt="You">
        </div>
    </div>
    
    <!-- Received message with multiple texts -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=5" alt="User">
        </div>
        <div class="ml-3 space-y-1">
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm inline-block">
                <p class="text-sm text-gray-700">I'm good too!</p>
            </div>
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm inline-block">
                <p class="text-sm text-gray-700">Do you want to grab lunch later today?</p>
            </div>
            <span class="text-xs text-gray-500 leading-none">10:18 AM</span>
        </div>
    </div>
</div>
```

## Example 2: Chat Bubbles with Status and Reactions

```html
<div class="flex flex-col space-y-4">
    <!-- Received message with reaction -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=3" alt="User">
        </div>
        <div class="ml-3">
            <div class="relative">
                <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm">
                    <p class="text-sm text-gray-700">Let's meet at the coffee shop at 3 PM.</p>
                </div>
                <div class="absolute -bottom-2 -right-2 flex -space-x-1">
                    <span class="flex items-center justify-center rounded-full border-2 border-white bg-gray-100 h-5 w-5">
                        <i class="ri-heart-fill text-xs text-red-500"></i>
                    </span>
                </div>
            </div>
            <div class="flex items-center mt-1">
                <span class="text-xs text-gray-500 leading-none">11:20 AM</span>
            </div>
        </div>
    </div>
    
    <!-- Sent message with status -->
    <div class="flex justify-end">
        <div class="mr-3">
            <div class="bg-blue-500 p-3 rounded-lg rounded-tr-none shadow-sm">
                <p class="text-sm text-white">Perfect! I'll be there. Should I bring the documents?</p>
            </div>
            <div class="flex items-center justify-end gap-1 mt-1">
                <span class="text-xs text-gray-500 leading-none">11:21 AM</span>
                <span>
                    <i class="ri-check-double-line text-blue-500"></i> <!-- Read status -->
                </span>
            </div>
        </div>
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=8" alt="You">
        </div>
    </div>
</div>
```

## Example 3: Different Bubble Types

```html
<div class="flex flex-col space-y-4">
    <!-- Image message -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=2" alt="User">
        </div>
        <div class="ml-3">
            <div class="bg-white rounded-lg rounded-tl-none shadow-sm overflow-hidden">
                <img src="https://images.unsplash.com/photo-1490730141103-6cac27aaab94?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=300&q=80" alt="Nature" class="w-full h-48 object-cover">
                <div class="p-3">
                    <p class="text-sm text-gray-700">Beautiful sunrise!</p>
                </div>
            </div>
            <span class="text-xs text-gray-500 leading-none">11:30 AM</span>
        </div>
    </div>
    
    <!-- File message -->
    <div class="flex justify-end">
        <div class="mr-3">
            <div class="bg-blue-500 p-3 rounded-lg rounded-tr-none shadow-sm">
                <div class="flex items-center bg-blue-600 rounded p-2 text-white">
                    <i class="ri-file-pdf-line text-xl mr-2"></i>
                    <div>
                        <p class="text-sm font-medium">Project_Report.pdf</p>
                        <p class="text-xs opacity-75">2.3 MB</p>
                    </div>
                    <i class="ri-download-line ml-3"></i>
                </div>
            </div>
            <span class="text-xs text-gray-500 leading-none flex justify-end">11:35 AM</span>
        </div>
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=8" alt="You">
        </div>
    </div>
    
    <!-- Audio message -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=2" alt="User">
        </div>
        <div class="ml-3">
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm">
                <div class="flex items-center">
                    <button class="flex-shrink-0 bg-gray-200 hover:bg-gray-300 rounded-full p-1.5">
                        <i class="ri-play-fill text-gray-600"></i>
                    </button>
                    <div class="ml-2 w-32">
                        <div class="h-1.5 bg-gray-200 rounded-full">
                            <div class="h-1.5 bg-gray-500 rounded-full w-1/3"></div>
                        </div>
                    </div>
                    <span class="ml-2 text-xs text-gray-500">0:18</span>
                </div>
            </div>
            <span class="text-xs text-gray-500 leading-none">11:40 AM</span>
        </div>
    </div>
</div>
```

## Example 4: Group Chat

```html
<div class="flex flex-col space-y-4">
    <!-- System message -->
    <div class="flex justify-center">
        <div class="bg-gray-200 px-3 py-1 rounded-full inline-block">
            <span class="text-xs text-gray-600">Today, 2:00 PM</span>
        </div>
    </div>
    
    <!-- First person message -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=1" alt="Alex">
        </div>
        <div class="ml-3">
            <div>
                <span class="text-xs font-semibold text-gray-800">Alex</span>
            </div>
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm">
                <p class="text-sm text-gray-700">Hey everyone! When is our next team meeting?</p>
            </div>
            <span class="text-xs text-gray-500 leading-none">2:05 PM</span>
        </div>
    </div>
    
    <!-- Second person message -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=2" alt="Sarah">
        </div>
        <div class="ml-3">
            <div>
                <span class="text-xs font-semibold text-gray-800">Sarah</span>
            </div>
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm">
                <p class="text-sm text-gray-700">I think it's tomorrow at 10 AM, isn't it?</p>
            </div>
            <span class="text-xs text-gray-500 leading-none">2:06 PM</span>
        </div>
    </div>
</div>
```

## Example 5: Chat Bubbles with Actions

```html
<div class="flex flex-col space-y-4">
    <!-- Message with link preview -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=4" alt="User">
        </div>
        <div class="ml-3">
            <div class="bg-white rounded-lg rounded-tl-none shadow-sm overflow-hidden">
                <div class="p-3">
                    <p class="text-sm text-gray-700">Check out this interesting article:</p>
                    <a href="#" class="text-blue-600 text-sm hover:underline">https://tailwindcss.com/blog/tailwindcss-v3</a>
                </div>
                <div class="border-t">
                    <div class="flex items-center p-3">
                        <div class="h-12 w-12 bg-blue-50 flex items-center justify-center rounded-lg flex-shrink-0">
                            <i class="ri-tailwind-fill text-blue-500 text-xl"></i>
                        </div>
                        <div class="ml-3">
                            <p class="text-sm font-medium text-gray-900">Tailwind CSS v3.0</p>
                            <p class="text-xs text-gray-500 truncate">The latest version of Tailwind CSS with incredible performance...</p>
                        </div>
                    </div>
                </div>
            </div>
            <span class="text-xs text-gray-500 leading-none">3:20 PM</span>
        </div>
    </div>
    
    <!-- Action buttons message -->
    <div class="flex">
        <div class="flex-shrink-0">
            <img class="h-8 w-8 rounded-full" src="https://i.pravatar.cc/100?img=4" alt="User">
        </div>
        <div class="ml-3">
            <div class="bg-white p-3 rounded-lg rounded-tl-none shadow-sm">
                <p class="text-sm text-gray-700 mb-3">Can you confirm your attendance for the team dinner?</p>
                <div class="flex flex-col space-y-2">
                    <button class="px-4 py-2 bg-blue-600 text-white text-sm font-medium rounded-md hover:bg-blue-700">Yes, I'll attend</button>
                    <button class="px-4 py-2 bg-gray-200 text-gray-700 text-sm font-medium rounded-md hover:bg-gray-300">No, I can't make it</button>
                    <button class="px-4 py-2 bg-gray-200 text-gray-700 text-sm font-medium rounded-md hover:bg-gray-300">Maybe, I'll let you know later</button>
                </div>
            </div>
            <span class="text-xs text-gray-500 leading-none">3:25 PM</span>
        </div>
    </div>
</div>
```
