# Form Component Examples

## Example 1: Contact Form

```html
<form class="max-w-2xl mx-auto">
    <div class="mb-6">
        <label for="name" class="block mb-2 text-sm font-medium text-gray-900">Your Name</label>
        <div class="relative">
            <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                <i class="ri-user-3-line text-gray-500"></i>
            </div>
            <input type="text" id="name" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" placeholder="John Doe" required>
        </div>
    </div>
    
    <div class="mb-6">
        <label for="email" class="block mb-2 text-sm font-medium text-gray-900">Your Email</label>
        <div class="relative">
            <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                <i class="ri-mail-line text-gray-500"></i>
            </div>
            <input type="email" id="email" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" placeholder="name@example.com" required>
        </div>
    </div>
    
    <div class="mb-6">
        <label for="subject" class="block mb-2 text-sm font-medium text-gray-900">Subject</label>
        <div class="relative">
            <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                <i class="ri-chat-1-line text-gray-500"></i>
            </div>
            <input type="text" id="subject" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" placeholder="Let us know how we can help you" required>
        </div>
    </div>
    
    <div class="mb-6">
        <label for="message" class="block mb-2 text-sm font-medium text-gray-900">Your Message</label>
        <textarea id="message" rows="4" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500" placeholder="Leave a comment..."></textarea>
    </div>
    
    <div class="mb-6">
        <div class="flex items-start">
            <div class="flex items-center h-5">
                <input id="remember" type="checkbox" value="" class="w-4 h-4 border border-gray-300 rounded bg-gray-50 focus:ring-3 focus:ring-blue-300" required>
            </div>
            <label for="remember" class="ml-2 text-sm font-medium text-gray-900">I agree to the <a href="#" class="text-blue-600 hover:underline">terms and conditions</a></label>
        </div>
    </div>
    
    <button type="submit" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center flex items-center mx-auto">
        <i class="ri-send-plane-fill mr-2"></i> Send Message
    </button>
</form>
```

## Example 2: Login Form with Social Login

```html
<form class="max-w-md mx-auto">
    <div class="flex justify-center mb-8">
        <div class="bg-blue-600 text-white rounded-full p-3">
            <i class="ri-lock-2-line text-3xl"></i>
        </div>
    </div>
    
    <h3 class="text-xl font-bold text-center mb-6 text-gray-800">Sign In to Your Account</h3>
    
    <div class="mb-6">
        <label for="login-email" class="block mb-2 text-sm font-medium text-gray-900">Email</label>
        <input type="email" id="login-email" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="name@example.com" required>
    </div>
    
    <div class="mb-6">
        <div class="flex justify-between mb-2">
            <label for="login-password" class="text-sm font-medium text-gray-900">Password</label>
            <a href="#" class="text-sm text-blue-600 hover:underline">Forgot password?</a>
        </div>
        <div class="relative">
            <input type="password" id="login-password" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 pr-10" required>
            <button type="button" class="absolute inset-y-0 right-0 flex items-center pr-3" onclick="togglePasswordVisibility()">
                <i class="ri-eye-line text-gray-500"></i>
            </button>
        </div>
    </div>
    
    <div class="mb-6">
        <div class="flex items-start">
            <div class="flex items-center h-5">
                <input id="remember-me" type="checkbox" value="" class="w-4 h-4 border border-gray-300 rounded bg-gray-50 focus:ring-3 focus:ring-blue-300">
            </div>
            <label for="remember-me" class="ml-2 text-sm font-medium text-gray-900">Remember me</label>
        </div>
    </div>
    
    <button type="submit" class="w-full text-white bg-blue-600 hover:bg-blue-700 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center mb-6">Sign In</button>
    
    <div class="flex items-center my-4">
        <hr class="flex-grow border-gray-300">
        <span class="px-3 text-gray-500 text-sm">Or continue with</span>
        <hr class="flex-grow border-gray-300">
    </div>
    
    <div class="grid grid-cols-3 gap-3 mb-6">
        <button type="button" class="py-2.5 px-5 text-sm font-medium text-gray-900 focus:outline-none bg-white rounded-lg border border-gray-200 hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:ring-gray-200 flex justify-center">
            <i class="ri-google-fill text-lg"></i>
        </button>
        <button type="button" class="py-2.5 px-5 text-sm font-medium text-gray-900 focus:outline-none bg-white rounded-lg border border-gray-200 hover:bg-gray-100 hover:text-[#1877F2] focus:z-10 focus:ring-4 focus:ring-gray-200 flex justify-center">
            <i class="ri-facebook-fill text-lg"></i>
        </button>
        <button type="button" class="py-2.5 px-5 text-sm font-medium text-gray-900 focus:outline-none bg-white rounded-lg border border-gray-200 hover:bg-gray-100 hover:text-[#1DA1F2] focus:z-10 focus:ring-4 focus:ring-gray-200 flex justify-center">
            <i class="ri-twitter-x-fill text-lg"></i>
        </button>
    </div>
    
    <div class="text-sm font-medium text-gray-500 text-center">
        Not registered? <a href="#" class="text-blue-600 hover:underline">Create account</a>
    </div>
</form>
```

## Example 3: Registration Form with Validation

```html
<form class="max-w-xl mx-auto space-y-6">
    <h3 class="text-xl font-bold text-center mb-4 text-gray-800">Create Your Account</h3>
    <p class="text-gray-500 text-center mb-6">Fill in the information below to get started</p>
    
    <div class="grid gap-6 mb-6 md:grid-cols-2">
        <div>
            <label for="first_name" class="block mb-2 text-sm font-medium text-gray-900">First name</label>
            <input type="text" id="first_name" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="John" required>
        </div>
        <div>
            <label for="last_name" class="block mb-2 text-sm font-medium text-gray-900">Last name</label>
            <input type="text" id="last_name" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="Doe" required>
        </div>
    </div>
    
    <div>
        <label for="register-email" class="block mb-2 text-sm font-medium text-gray-900">Email address</label>
        <input type="email" id="register-email" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="john.doe@company.com" required>
        <p class="mt-1 text-sm text-green-600">Email format is valid</p>
    </div>
    
    <div>
        <label for="register-password" class="block mb-2 text-sm font-medium text-gray-900">Password</label>
        <input type="password" id="register-password" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="•••••••••" required>
    </div>
    
    <div>
        <label for="confirm-password" class="block mb-2 text-sm font-medium text-gray-900">Confirm password</label>
        <input type="password" id="confirm-password" class="bg-gray-50 border border-red-500 text-gray-900 text-sm rounded-lg focus:ring-red-500 focus:border-red-500 block w-full p-2.5" placeholder="•••••••••" required>
        <p class="mt-1 text-sm text-red-600">Passwords don't match</p>
    </div>
    
    <div>
        <label for="phone" class="block mb-2 text-sm font-medium text-gray-900">Phone number</label>
        <input type="tel" id="phone" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="123-456-7890" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" required>
    </div>
    
    <div class="flex items-start">
        <div class="flex items-center h-5">
            <input id="terms" type="checkbox" class="w-4 h-4 border border-gray-300 rounded bg-gray-50 focus:ring-3 focus:ring-blue-300" required>
        </div>
        <label for="terms" class="ml-2 text-sm font-medium text-gray-900">I agree with the <a href="#" class="text-blue-600 hover:underline">terms and conditions</a></label>
    </div>
    
    <div>
        <label class="block mb-2 text-sm font-medium text-gray-900">Security Level</label>
        <div class="w-full bg-gray-200 rounded-full h-2.5 mb-2">
            <div class="bg-red-500 h-2.5 rounded-full" style="width: 33%"></div>
        </div>
        <p class="text-sm text-red-600">Weak - Add numbers and symbols</p>
    </div>
    
    <button type="submit" class="w-full text-white bg-blue-600 hover:bg-blue-700 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center">Register</button>
    
    <div class="text-sm font-medium text-gray-500 text-center">
        Already have an account? <a href="#" class="text-blue-600 hover:underline">Sign in here</a>
    </div>
</form>
```

## Example 4: Multi-Step Form

```html
<div class="max-w-2xl mx-auto">
    <!-- Progress Bar -->
    <div class="mb-8">
        <div class="flex items-center justify-between mb-2">
            <span class="text-sm font-medium text-blue-600">Step 2 of 3</span>
            <span class="text-sm font-medium text-gray-500">Personal Details</span>
        </div>
        <div class="w-full bg-gray-200 rounded-full h-2.5">
            <div class="bg-blue-600 h-2.5 rounded-full" style="width: 66%"></div>
        </div>
    </div>
    
    <!-- Step Indicators -->
    <div class="flex items-center justify-between mb-8">
        <div class="flex flex-col items-center">
            <div class="w-10 h-10 bg-blue-100 text-blue-600 rounded-full flex items-center justify-center border-2 border-blue-600">
                <i class="ri-check-line text-xl"></i>
            </div>
            <span class="text-xs font-medium text-gray-500 mt-2">Account</span>
        </div>
        <div class="flex-grow border-t-2 border-blue-600 mx-2"></div>
        <div class="flex flex-col items-center">
            <div class="w-10 h-10 bg-blue-600 text-white rounded-full flex items-center justify-center border-2 border-blue-600">
                <span class="text-sm font-bold">2</span>
            </div>
            <span class="text-xs font-medium text-gray-500 mt-2">Personal</span>
        </div>
        <div class="flex-grow border-t-2 border-gray-300 mx-2"></div>
        <div class="flex flex-col items-center">
            <div class="w-10 h-10 bg-white text-gray-500 rounded-full flex items-center justify-center border-2 border-gray-300">
                <span class="text-sm font-bold">3</span>
            </div>
            <span class="text-xs font-medium text-gray-500 mt-2">Complete</span>
        </div>
    </div>
    
    <!-- Form Fields for Current Step -->
    <form class="space-y-6">
        <h3 class="text-xl font-semibold text-center mb-6">Personal Information</h3>
        
        <div>
            <label for="full-name" class="block mb-2 text-sm font-medium text-gray-900">Full Name</label>
            <input type="text" id="full-name" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" required>
        </div>
        
        <div>
            <label for="date-of-birth" class="block mb-2 text-sm font-medium text-gray-900">Date of Birth</label>
            <div class="relative">
                <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                    <i class="ri-calendar-line text-gray-500"></i>
                </div>
                <input type="date" id="date-of-birth" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" required>
            </div>
        </div>
        
        <div>
            <label for="phone-number" class="block mb-2 text-sm font-medium text-gray-900">Phone Number</label>
            <div class="relative">
                <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                    <i class="ri-phone-line text-gray-500"></i>
                </div>
                <input type="tel" id="phone-number" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" placeholder="(123) 456-7890" required>
            </div>
        </div>
        
        <div class="flex justify-between pt-4">
            <button type="button" class="py-2.5 px-5 text-sm font-medium text-gray-900 focus:outline-none bg-white rounded-lg border border-gray-200 hover:bg-gray-100 hover:text-blue-700 focus:z-10 focus:ring-4 focus:ring-gray-200 flex items-center">
                <i class="ri-arrow-left-s-line mr-1"></i> Previous
            </button>
            <button type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 flex items-center">
                Next <i class="ri-arrow-right-s-line ml-1"></i>
            </button>
        </div>
    </form>
</div>
```

## Example 5: Payment Form

```html
<div class="max-w-lg mx-auto">
    <form class="space-y-6">
        <div class="bg-blue-50 border border-blue-200 rounded-lg p-4 flex items-start mb-6">
            <i class="ri-secure-payment-line text-blue-500 text-xl mt-0.5 mr-3"></i>
            <div>
                <h4 class="font-semibold text-blue-800">Secure Payment</h4>
                <p class="text-blue-700 text-sm">Your payment information is encrypted and secure.</p>
            </div>
        </div>
        
        <div>
            <label class="block mb-3 text-sm font-medium text-gray-900">Payment Method</label>
            <div class="grid grid-cols-4 gap-2">
                <div>
                    <input type="radio" name="payment_type" id="type-card" value="card" class="hidden peer" checked>
                    <label for="type-card" class="flex flex-col items-center justify-center p-4 text-gray-500 bg-white border border-gray-200 rounded-lg cursor-pointer peer-checked:border-blue-600 peer-checked:text-blue-600 hover:bg-gray-50">
                        <i class="ri-bank-card-line text-2xl mb-2"></i>
                        <div class="w-full text-xs font-semibold text-center">Credit Card</div>
                    </label>
                </div>
                <div>
                    <input type="radio" name="payment_type" id="type-paypal" value="paypal" class="hidden peer">
                    <label for="type-paypal" class="flex flex-col items-center justify-center p-4 text-gray-500 bg-white border border-gray-200 rounded-lg cursor-pointer peer-checked:border-blue-600 peer-checked:text-blue-600 hover:bg-gray-50">
                        <i class="ri-paypal-line text-2xl mb-2"></i>
                        <div class="w-full text-xs font-semibold text-center">PayPal</div>
                    </label>
                </div>
                <div>
                    <input type="radio" name="payment_type" id="type-apple" value="apple" class="hidden peer">
                    <label for="type-apple" class="flex flex-col items-center justify-center p-4 text-gray-500 bg-white border border-gray-200 rounded-lg cursor-pointer peer-checked:border-blue-600 peer-checked:text-blue-600 hover:bg-gray-50">
                        <i class="ri-apple-fill text-2xl mb-2"></i>
                        <div class="w-full text-xs font-semibold text-center">Apple Pay</div>
                    </label>
                </div>
                <div>
                    <input type="radio" name="payment_type" id="type-google" value="google" class="hidden peer">
                    <label for="type-google" class="flex flex-col items-center justify-center p-4 text-gray-500 bg-white border border-gray-200 rounded-lg cursor-pointer peer-checked:border-blue-600 peer-checked:text-blue-600 hover:bg-gray-50">
                        <i class="ri-google-fill text-2xl mb-2"></i>
                        <div class="w-full text-xs font-semibold text-center">Google Pay</div>
                    </label>
                </div>
            </div>
        </div>
        
        <!-- Credit Card Details -->
        <div id="credit-card-details">
            <div class="space-y-4">
                <div>
                    <label for="card-holder" class="block mb-2 text-sm font-medium text-gray-900">Card Holder Name</label>
                    <input type="text" id="card-holder" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="As shown on card" required>
                </div>
                
                <div>
                    <label for="card-number" class="block mb-2 text-sm font-medium text-gray-900">Card Number</label>
                    <div class="relative">
                        <input type="text" id="card-number" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 pr-10" placeholder="1234 5678 9012 3456" required>
                        <div class="absolute inset-y-0 right-0 flex items-center pr-3 pointer-events-none">
                            <i class="ri-visa-line text-blue-700 text-xl"></i>
                        </div>
                    </div>
                </div>
                
                <div class="grid grid-cols-2 gap-6">
                    <div>
                        <label for="expiry-date" class="block mb-2 text-sm font-medium text-gray-900">Expiry Date</label>
                        <input type="text" id="expiry-date" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="MM/YY" required>
                    </div>
                    <div>
                        <label for="security-code" class="block mb-2 text-sm font-medium text-gray-900">
                            <div class="flex items-center">
                                <span>Security Code</span>
                                <button type="button" class="ml-2 text-gray-400 hover:text-gray-500" title="3-digit code on back of your card">
                                    <i class="ri-question-line"></i>
                                </button>
                            </div>
                        </label>
                        <input type="text" id="security-code" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5" placeholder="CVV" required>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="border-t border-gray-200 pt-6">
            <div class="flex justify-between mb-2">
                <span class="text-base font-medium text-gray-900">Subtotal</span>
                <span class="text-base font-medium text-gray-900">$99.00</span>
            </div>
            <div class="flex justify-between mb-2">
                <span class="text-sm text-gray-500">Tax</span>
                <span class="text-sm text-gray-500">$8.91</span>
            </div>
            <div class="flex justify-between font-semibold text-lg pt-4 border-t">
                <span>Total</span>
                <span>$107.91</span>
            </div>
        </div>
        
        <button type="submit" class="w-full text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-base px-5 py-3 text-center flex items-center justify-center">
            <i class="ri-lock-line mr-2"></i> Pay $107.91
        </button>
    </form>
</div>
```

## JavaScript for Password Toggle

```javascript
function togglePasswordVisibility() {
    const passwordInput = document.getElementById("login-password");
    const icon = document.querySelector("#login-password + button i");
    
    if (passwordInput.type === "password") {
        passwordInput.type = "text";
        icon.classList.replace("ri-eye-line", "ri-eye-off-line");
    } else {
        passwordInput.type = "password";
        icon.classList.replace("ri-eye-off-line", "ri-eye-line");
    }
}
```
