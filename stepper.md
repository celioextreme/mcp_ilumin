# Stepper Examples with Tailwind CSS and Remix Icon

## Example 1: Basic Horizontal Stepper

```html
<ol class="flex items-center w-full text-sm font-medium text-center text-gray-500 sm:text-base">
    <li class="flex md:w-full items-center text-blue-600 sm:after:content-[''] after:w-full after:h-1 after:border-b after:border-gray-200 after:border-1 after:hidden sm:after:inline-block after:mx-6 xl:after:mx-10">
        <span class="flex items-center justify-center w-8 h-8 bg-blue-100 rounded-full lg:h-10 lg:w-10 shrink-0">
            <i class="ri-check-line w-5 h-5 text-blue-600"></i>
        </span>
        <span class="hidden sm:inline-flex sm:ml-2">Personal Info</span>
    </li>
    <li class="flex md:w-full items-center text-blue-600 sm:after:content-[''] after:w-full after:h-1 after:border-b after:border-gray-200 after:border-1 after:hidden sm:after:inline-block after:mx-6 xl:after:mx-10">
        <span class="flex items-center justify-center w-8 h-8 bg-blue-100 rounded-full lg:h-10 lg:w-10 shrink-0">
            <i class="ri-check-line w-5 h-5 text-blue-600"></i>
        </span>
        <span class="hidden sm:inline-flex sm:ml-2">Account Details</span>
    </li>
    <li class="flex md:w-full items-center after:content-[''] after:w-full after:h-1 after:border-b after:border-gray-200 after:border-1 after:hidden sm:after:inline-block after:mx-6 xl:after:mx-10">
        <span class="flex items-center justify-center w-8 h-8 bg-gray-100 rounded-full lg:h-10 lg:w-10 shrink-0">
            <span class="text-gray-600">3</span>
        </span>
        <span class="hidden sm:inline-flex sm:ml-2">Review</span>
    </li>
</ol>
```

## Example 2: Numbered Vertical Stepper

```html
<ol class="space-y-6">
    <li class="relative">
        <div class="flex items-start">
            <div class="flex items-center justify-center w-10 h-10 bg-blue-600 rounded-full text-white font-bold text-lg shrink-0">
                1
            </div>
            <div class="ml-4">
                <h3 class="text-lg font-semibold text-gray-900">Complete Your Profile</h3>
                <p class="text-gray-600 mt-1">Fill in your personal information to get started.</p>
                <div class="mt-4 bg-gray-50 border border-gray-200 rounded-lg p-4">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label class="block mb-2 text-sm font-medium text-gray-900">First Name</label>
                            <input type="text" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                        </div>
                        <div>
                            <label class="block mb-2 text-sm font-medium text-gray-900">Last Name</label>
                            <input type="text" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="absolute top-10 left-5 h-full border-l-2 border-gray-200"></div>
    </li>
</ol>
```

## Example 3: Interactive Progress Stepper

```html
<div class="mb-8">
    <div class="flex items-center justify-between mb-4">
        <div class="w-full h-2 bg-gray-200 rounded-full">
            <div id="progress-bar" class="h-2 bg-blue-600 rounded-full transition-all duration-300" style="width: 0%"></div>
        </div>
    </div>
    <div class="flex justify-between">
        <div class="flex flex-col items-center">
            <button id="step1-btn" class="w-10 h-10 flex items-center justify-center rounded-full bg-blue-600 text-white font-bold mb-2">
                <i class="ri-user-line text-lg"></i>
            </button>
            <span class="text-xs text-blue-600 font-semibold">Profile</span>
        </div>
        <div class="flex flex-col items-center">
            <button id="step2-btn" class="w-10 h-10 flex items-center justify-center rounded-full bg-gray-300 text-gray-600 font-bold mb-2">
                <i class="ri-settings-3-line text-lg"></i>
            </button>
            <span class="text-xs text-gray-500 font-semibold">Settings</span>
        </div>
    </div>
</div>

<script>
    // JavaScript for Interactive Progress Stepper
    document.addEventListener('DOMContentLoaded', function() {
        const progressBar = document.getElementById('progress-bar');
        const prevBtn = document.getElementById('prev-btn');
        const nextBtn = document.getElementById('next-btn');
        const stepButtons = [
            document.getElementById('step1-btn'),
            document.getElementById('step2-btn'),
            document.getElementById('step3-btn'),
            document.getElementById('step4-btn')
        ];
        const stepContents = [
            document.getElementById('step1-content'),
            document.getElementById('step2-content'),
            document.getElementById('step3-content'),
            document.getElementById('step4-content')
        ];
        
        let currentStep = 0;
        
        function updateStep(step) {
            // Update progress bar
            const progressPercentage = (step / (stepButtons.length - 1)) * 100;
            progressBar.style.width = `${progressPercentage}%`;
            
            // Update buttons state and step content visibility
            // ... (additional update logic)
        }
        
        // Add event listeners and initialize
    });
</script>
```

## Example 4: Stepper with Progress Line

```html
<div class="max-w-3xl mx-auto">
    <div class="flex items-center">
        <div class="flex items-center relative">
            <div class="rounded-full transition duration-500 ease-in-out h-12 w-12 py-3 border-2 bg-blue-600 border-blue-600 text-white flex items-center justify-center">
                <i class="ri-shopping-cart-line text-lg"></i>
            </div>
            <div class="absolute top-0 -ml-10 text-center mt-16 w-32 text-xs font-medium text-blue-600">Shopping Cart</div>
        </div>
        <div class="flex-auto border-t-2 transition duration-500 ease-in-out border-blue-600"></div>
        <div class="flex items-center relative">
            <div class="rounded-full transition duration-500 ease-in-out h-12 w-12 py-3 border-2 bg-blue-600 border-blue-600 text-white flex items-center justify-center">
                <i class="ri-map-pin-line text-lg"></i>
            </div>
            <div class="absolute top-0 -ml-10 text-center mt-16 w-32 text-xs font-medium text-blue-600">Shipping</div>
        </div>
        <div class="flex-auto border-t-2 transition duration-500 ease-in-out border-gray-300"></div>
        <div class="flex items-center relative">
            <div class="rounded-full transition duration-500 ease-in-out h-12 w-12 py-3 border-2 border-gray-300 text-gray-500 flex items-center justify-center">
                <i class="ri-bank-card-line text-lg"></i>
            </div>
            <div class="absolute top-0 -ml-10 text-center mt-16 w-32 text-xs font-medium text-gray-500">Payment</div>
        </div>
    </div>
</div>
```

## Example 5: Wizard Stepper with Form Validation

```html
<!-- Stepper Header -->
<div class="mb-8">
    <div class="relative after:absolute after:inset-x-0 after:top-1/2 after:-translate-y-1/2 after:h-0.5 after:bg-gray-200 after:z-[1]">
        <ol class="relative z-[2] flex justify-between">
            <li class="flex items-center justify-center w-8 h-8 rounded-full bg-blue-600 text-white font-medium">
                1
            </li>
            <li class="flex items-center justify-center w-8 h-8 rounded-full bg-gray-200 text-gray-600 font-medium">
                2
            </li>
            <li class="flex items-center justify-center w-8 h-8 rounded-full bg-gray-200 text-gray-600 font-medium">
                3
            </li>
        </ol>
    </div>
    <div class="flex justify-between mt-2">
        <span class="text-sm font-medium text-blue-600">Registration</span>
        <span class="text-sm font-medium text-gray-500">Company Details</span>
        <span class="text-sm font-medium text-gray-500">Confirmation</span>
    </div>
</div>

<script>
    // Form validation code
    function validateStep(step) {
        if (step === 0) {
            const emailInput = document.getElementById('email');
            const emailError = document.getElementById('email-error');
            
            let isValid = true;
            
            // Simple email validation
            if (!emailInput.value || !emailInput.value.includes('@')) {
                emailError.classList.remove('hidden');
                isValid = false;
            } else {
                emailError.classList.add('hidden');
            }
            
            // Additional validation logic...
            
            return isValid;
        }
        
        return true;
    }
</script>
```
