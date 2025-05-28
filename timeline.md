# Timeline Examples with Tailwind CSS and Remix Icon

## Example 1: Basic Vertical Timeline

```html
<ol class="relative border-l border-gray-200 ml-3">
    <li class="mb-10 ml-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -left-3 ring-8 ring-white">
            <i class="ri-file-list-line text-blue-800"></i>
        </span>
        <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900">Project Kickoff</h3>
        <time class="block mb-2 text-sm font-normal leading-none text-gray-400">January 13, 2023</time>
        <p class="mb-4 text-base font-normal text-gray-500">Initial project planning and team onboarding completed. Requirements gathered and project scope defined.</p>
        <a href="#" class="inline-flex items-center px-4 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-200 rounded-lg hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-2 focus:ring-blue-700 focus:text-blue-700">
            <i class="ri-file-list-3-line mr-2"></i> View Documentation
        </a>
    </li>
    
    <li class="mb-10 ml-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-green-100 rounded-full -left-3 ring-8 ring-white">
            <i class="ri-code-s-slash-line text-green-800"></i>
        </span>
        <h3 class="mb-1 text-lg font-semibold text-gray-900">Development Phase</h3>
        <time class="block mb-2 text-sm font-normal leading-none text-gray-400">March 7, 2023</time>
        <p class="text-base font-normal text-gray-500">Core functionality implemented. Initial testing phase started.</p>
    </li>
</ol>
```

## Example 2: Horizontal Timeline

```html
<div class="min-w-[800px]">
    <!-- Timeline Track -->
    <div class="relative">
        <!-- Timeline Line -->
        <div class="absolute h-0.5 w-full bg-gray-200 top-5 z-0"></div>
        
        <!-- Timeline Items -->
        <ol class="flex justify-between relative">
            <!-- Item 1 -->
            <li class="relative mb-6 w-1/4">
                <div class="flex items-center">
                    <div class="z-10 flex items-center justify-center w-10 h-10 bg-blue-600 rounded-full ring-0 ring-white sm:ring-8 shrink-0">
                        <i class="ri-flag-2-line text-white"></i>
                    </div>
                    <div class="hidden sm:flex w-full bg-gray-200 h-0.5"></div>
                </div>
                <div class="mt-3">
                    <h3 class="text-lg font-semibold text-gray-900">Planning</h3>
                    <time class="block mb-2 text-sm font-normal leading-none text-gray-400">Q1 2023</time>
                    <p class="text-base font-normal text-gray-500 max-w-[150px]">Project definition and scope planning.</p>
                </div>
            </li>
            
            <!-- Item 2 -->
            <li class="relative mb-6 w-1/4">
                <div class="flex items-center">
                    <div class="z-10 flex items-center justify-center w-10 h-10 bg-blue-600 rounded-full ring-0 ring-white sm:ring-8 shrink-0">
                        <i class="ri-pencil-ruler-2-line text-white"></i>
                    </div>
                    <div class="hidden sm:flex w-full bg-gray-200 h-0.5"></div>
                </div>
                <div class="mt-3">
                    <h3 class="text-lg font-semibold text-gray-900">Design</h3>
                    <time class="block mb-2 text-sm font-normal leading-none text-gray-400">Q2 2023</time>
                    <p class="text-base font-normal text-gray-500 max-w-[150px]">UI/UX design and prototyping.</p>
                </div>
            </li>
        </ol>
    </div>
</div>
```

## Example 3: Activity Timeline

```html
<div class="flow-root">
    <ul role="list" class="space-y-6">
        <li class="relative flex gap-x-4">
            <div class="absolute left-0 top-0 flex w-6 justify-center -bottom-6">
                <div class="w-px bg-gray-200"></div>
            </div>
            <div class="relative flex h-6 w-6 flex-none items-center justify-center bg-white">
                <div class="h-1.5 w-1.5 rounded-full bg-gray-100 ring-1 ring-gray-300"></div>
            </div>
            <p class="flex-auto py-0.5 text-xs leading-5 text-gray-500">
                <span class="font-medium text-gray-900">Today</span>
            </p>
            <time datetime="2023-01-23T10:32" class="flex-none py-0.5 text-xs leading-5 text-gray-500">10:32 AM</time>
        </li>
        
        <li class="relative flex gap-x-4">
            <div class="absolute left-0 top-0 flex w-6 justify-center -bottom-6">
                <div class="w-px bg-gray-200"></div>
            </div>
            <div class="relative flex h-6 w-6 flex-none items-center justify-center bg-white">
                <div class="h-3 w-3 rounded-full bg-blue-500"></div>
            </div>
            <p class="flex-auto py-0.5 text-sm leading-5 text-gray-500">
                <span class="font-medium text-gray-900">Alex Johnson</span> commented on <span class="font-medium text-gray-900">Design Review</span>
            </p>
            <time datetime="2023-01-23T09:12" class="flex-none py-0.5 text-xs leading-5 text-gray-500">9:12 AM</time>
        </li>
    </ul>
</div>
```

## Example 4: Timeline with Alternating Sides

```html
<div class="container mx-auto w-full">
    <!-- Timeline center line -->
    <div class="relative wrap overflow-hidden p-4 h-full">
        <div class="absolute h-full border-2 border-dashed border-gray-200 left-1/2"></div>
        
        <!-- Right side -->
        <div class="flex justify-between items-center w-full mb-8 right-timeline">
            <div class="order-1 w-5/12"></div>
            <div class="z-10 flex items-center order-1 bg-blue-500 shadow-xl w-8 h-8 rounded-full">
                <h1 class="mx-auto font-semibold text-lg text-white">1</h1>
            </div>
            <div class="order-1 bg-blue-50 rounded-lg shadow-xl w-5/12 px-6 py-4">
                <h3 class="font-bold text-gray-800 text-lg">Company Founded</h3>
                <p class="text-sm text-gray-500 mt-1">January 2020</p>
                <p class="text-sm leading-snug tracking-wide text-gray-600 mt-2">The journey begins with three founders and a vision to change the industry.</p>
            </div>
        </div>

        <!-- Left side -->
        <div class="flex justify-between items-center w-full mb-8 left-timeline">
            <div class="order-1 bg-purple-50 rounded-lg shadow-xl w-5/12 px-6 py-4">
                <h3 class="font-bold text-gray-800 text-lg">First Major Client</h3>
                <p class="text-sm text-gray-500 mt-1">March 2020</p>
                <p class="text-sm leading-snug tracking-wide text-gray-600 mt-2">Secured our first enterprise client and proved our business model.</p>
            </div>
            <div class="z-10 flex items-center order-1 bg-purple-500 shadow-xl w-8 h-8 rounded-full">
                <h1 class="mx-auto font-semibold text-lg text-white">2</h1>
            </div>
            <div class="order-1 w-5/12"></div>
        </div>
    </div>
</div>
```

## Example 5: Interactive Timeline with Expandable Content

```html
<ol class="relative border-l border-gray-200 ml-3">
    <li class="mb-10 ml-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -left-3 ring-8 ring-white">
            <i class="ri-file-list-line text-blue-800"></i>
        </span>
        <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900">
            Product Conception
            <span class="bg-blue-100 text-blue-800 text-sm font-medium mr-2 px-2.5 py-0.5 rounded ml-3">Latest</span>
        </h3>
        <time class="block mb-2 text-sm font-normal leading-none text-gray-400">January 10, 2023</time>
        <div class="mb-4 text-base font-normal text-gray-500">
            <p class="mb-2">Initial product ideas formed and market research conducted.</p>
            <button class="timeline-expand-btn text-blue-600 hover:underline flex items-center" data-target="content-1">
                <span>Read more</span>
                <i class="ri-arrow-down-s-line ml-1"></i>
            </button>
            <div id="content-1" class="hidden mt-3 bg-gray-50 p-4 rounded-lg">
                <h4 class="text-base font-medium mb-2">Market Research Findings</h4>
                <ul class="list-disc pl-5 mb-3 text-sm space-y-1">
                    <li>Identified 3 key competitors in the space</li>
                    <li>Discovered unmet needs in the target market</li>
                    <li>Initial target audience defined: 25-45 year old professionals</li>
                </ul>
                <p class="text-sm">Team conducted 12 user interviews and analyzed 5 competing products to identify opportunities for differentiation.</p>
            </div>
        </div>
    </li>
</ol>

<!-- JavaScript for Expandable Content -->
<script>
    document.querySelectorAll('.timeline-expand-btn').forEach(button => {
        button.addEventListener('click', function() {
            const targetId = this.getAttribute('data-target');
            const targetContent = document.getElementById(targetId);
            
            // Toggle the content visibility
            targetContent.classList.toggle('hidden');
            
            // Update the button text and icon
            const buttonText = this.querySelector('span');
            const buttonIcon = this.querySelector('i');
            
            if (targetContent.classList.contains('hidden')) {
                buttonIcon.classList.replace('ri-arrow-up-s-line', 'ri-arrow-down-s-line');
                buttonText.textContent = 'Read more';
            } else {
                buttonIcon.classList.replace('ri-arrow-down-s-line', 'ri-arrow-up-s-line');
                buttonText.textContent = 'Hide';
            }
        });
    });
</script>
```
