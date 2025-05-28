# Alert Examples

## Example 1: Success Notification Alert
Use this for successful operations like payments, form submissions, etc.

```html
<div class="flex items-center p-6 mb-4 text-green-800 border border-green-300 rounded-2xl bg-gradient-to-r from-green-50 to-green-100 dark:bg-gradient-to-r dark:from-gray-800 dark:to-gray-700 dark:text-green-400 dark:border-green-800 shadow-lg transform hover:scale-105 transition-all duration-300" role="alert">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center w-12 h-12 bg-green-500 rounded-full">
            <i class="ri-check-line text-2xl text-white"></i>
        </div>
    </div>
    <div class="ml-4 flex-1">
        <h3 class="text-lg font-bold mb-1">Payment Successful!</h3>
        <p class="text-sm">Your transaction has been completed successfully. Receipt sent to your email.</p>
    </div>
    <button type="button" class="ml-4 -mx-1.5 -my-1.5 bg-green-50 text-green-500 rounded-lg focus:ring-2 focus:ring-green-400 p-1.5 hover:bg-green-200 inline-flex items-center justify-center h-8 w-8 dark:bg-gray-800 dark:text-green-400 dark:hover:bg-gray-700 transition-colors duration-200" onclick="dismissAlert('success-alert')" aria-label="Close">
        <i class="ri-close-line text-lg"></i>
    </button>
</div>
```

## Example 2: Error/Danger Alert
Use this for error messages, failed operations, or critical issues.

```html
<div class="flex items-center p-6 mb-4 text-red-800 border border-red-300 rounded-2xl bg-gradient-to-r from-red-50 to-red-100 dark:bg-gradient-to-r dark:from-gray-800 dark:to-gray-700 dark:text-red-400 dark:border-red-800 shadow-lg transform hover:scale-105 transition-all duration-300" role="alert">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center w-12 h-12 bg-red-500 rounded-full animate-pulse">
            <i class="ri-error-warning-line text-2xl text-white"></i>
        </div>
    </div>
    <div class="ml-4 flex-1">
        <h3 class="text-lg font-bold mb-1">Error Occurred!</h3>
        <p class="text-sm mb-2">Failed to process your request. Please check your connection and try again.</p>
        <div class="flex space-x-2">
            <button class="text-xs bg-red-600 hover:bg-red-700 text-white px-3 py-1 rounded-lg transition-colors duration-200">
                <i class="ri-refresh-line mr-1"></i>Retry
            </button>
            <button class="text-xs bg-transparent border border-red-600 text-red-600 hover:bg-red-600 hover:text-white px-3 py-1 rounded-lg transition-colors duration-200">
                <i class="ri-customer-service-line mr-1"></i>Contact Support
            </button>
        </div>
    </div>
    <button type="button" class="ml-4 -mx-1.5 -my-1.5 bg-red-50 text-red-500 rounded-lg focus:ring-2 focus:ring-red-400 p-1.5 hover:bg-red-200 inline-flex items-center justify-center h-8 w-8 dark:bg-gray-800 dark:text-red-400 dark:hover:bg-gray-700 transition-colors duration-200" onclick="dismissAlert('error-alert')" aria-label="Close">
        <i class="ri-close-line text-lg"></i>
    </button>
</div>
```

## Example 3: Warning Alert
Use this for warnings, storage limits, or important notices that need attention.

```html
<div class="flex items-start p-6 mb-4 text-yellow-800 border border-yellow-300 rounded-2xl bg-gradient-to-r from-yellow-50 to-orange-50 dark:bg-gradient-to-r dark:from-gray-800 dark:to-gray-700 dark:text-yellow-300 dark:border-yellow-800 shadow-lg transform hover:scale-105 transition-all duration-300" role="alert">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center w-12 h-12 bg-yellow-500 rounded-full">
            <i class="ri-alert-line text-2xl text-white"></i>
        </div>
    </div>
    <div class="ml-4 flex-1">
        <h3 class="text-lg font-bold mb-1">Storage Almost Full!</h3>
        <p class="text-sm mb-3">You're using 89% of your storage space. Consider upgrading your plan or cleaning up files.</p>
        <div class="w-full bg-yellow-200 rounded-full h-2 mb-3 dark:bg-gray-600">
            <div class="bg-yellow-600 h-2 rounded-full" style="width: 89%"></div>
        </div>
        <ul class="text-xs space-y-1 mb-3">
            <li class="flex items-center"><i class="ri-file-line mr-2"></i>Delete unnecessary files</li>
            <li class="flex items-center"><i class="ri-upload-cloud-line mr-2"></i>Move files to cloud storage</li>
            <li class="flex items-center"><i class="ri-vip-crown-line mr-2"></i>Upgrade to premium plan</li>
        </ul>
        <button class="text-xs bg-yellow-600 hover:bg-yellow-700 text-white px-4 py-2 rounded-lg transition-colors duration-200">
            <i class="ri-settings-line mr-1"></i>Manage Storage
        </button>
    </div>
    <button type="button" class="ml-4 -mx-1.5 -my-1.5 bg-yellow-50 text-yellow-500 rounded-lg focus:ring-2 focus:ring-yellow-400 p-1.5 hover:bg-yellow-200 inline-flex items-center justify-center h-8 w-8 dark:bg-gray-800 dark:text-yellow-300 dark:hover:bg-gray-700 transition-colors duration-200" onclick="dismissAlert('warning-alert')" aria-label="Close">
        <i class="ri-close-line text-lg"></i>
    </button>
</div>
```

## Example 4: Info Alert
Use this for informational messages, feature announcements, or helpful tips.

```html
<div class="flex items-center p-6 mb-4 text-blue-800 border border-blue-300 rounded-2xl bg-gradient-to-r from-blue-50 to-cyan-50 dark:bg-gradient-to-r dark:from-gray-800 dark:to-gray-700 dark:text-blue-400 dark:border-blue-800 shadow-lg transform hover:scale-105 transition-all duration-300" role="alert">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center w-12 h-12 bg-blue-500 rounded-full">
            <i class="ri-information-line text-2xl text-white"></i>
        </div>
    </div>
    <div class="ml-4 flex-1">
        <h3 class="text-lg font-bold mb-1">New Feature Available!</h3>
        <p class="text-sm mb-3">We've added dark mode support to improve your experience. Try it out by clicking the theme toggle.</p>
        <div class="flex items-center space-x-4">
            <a href="#" class="text-blue-600 hover:text-blue-800 dark:text-blue-400 dark:hover:text-blue-300 text-sm font-medium inline-flex items-center transition-colors duration-200">
                <i class="ri-external-link-line mr-1"></i>Learn More
            </a>
            <span class="text-xs text-gray-500 dark:text-gray-400">
                <i class="ri-time-line mr-1"></i>2 minutes ago
            </span>
        </div>
    </div>
    <button type="button" class="ml-4 -mx-1.5 -my-1.5 bg-blue-50 text-blue-500 rounded-lg focus:ring-2 focus:ring-blue-400 p-1.5 hover:bg-blue-200 inline-flex items-center justify-center h-8 w-8 dark:bg-gray-800 dark:text-blue-400 dark:hover:bg-gray-700 transition-colors duration-200" onclick="dismissAlert('info-alert')" aria-label="Close">
        <i class="ri-close-line text-lg"></i>
    </button>
</div>
```

## Example 5: Security Alert
Use this for security notifications, login alerts, or account-related warnings.

```html
<div class="flex items-start p-6 mb-4 text-purple-800 border border-purple-300 rounded-2xl bg-gradient-to-r from-purple-50 to-pink-50 dark:bg-gradient-to-r dark:from-gray-800 dark:to-gray-700 dark:text-purple-400 dark:border-purple-800 shadow-lg transform hover:scale-105 transition-all duration-300" role="alert">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center w-12 h-12 bg-purple-500 rounded-full">
            <i class="ri-shield-check-line text-2xl text-white"></i>
        </div>
    </div>
    <div class="ml-4 flex-1">
        <h3 class="text-lg font-bold mb-1">Security Notice</h3>
        <p class="text-sm mb-3">We detected a new login from an unrecognized device. If this wasn't you, please secure your account immediately.</p>
        <div class="bg-purple-100 dark:bg-gray-700 rounded-lg p-3 mb-3">
            <div class="flex items-center justify-between text-xs">
                <span class="flex items-center">
                    <i class="ri-device-line mr-2"></i>Chrome on Windows
                </span>
                <span class="flex items-center">
                    <i class="ri-map-pin-line mr-1"></i>New York, US
                </span>
            </div>
            <div class="flex items-center justify-between text-xs mt-1">
                <span class="flex items-center">
                    <i class="ri-calendar-line mr-1"></i>Today, 2:30 PM
                </span>
                <span class="flex items-center">
                    <i class="ri-wifi-line mr-1"></i>192.168.1.105
                </span>
            </div>
        </div>
        <div class="flex space-x-2">
            <button class="text-xs bg-purple-600 hover:bg-purple-700 text-white px-3 py-1.5 rounded-lg transition-colors duration-200">
                <i class="ri-lock-line mr-1"></i>Secure Account
            </button>
            <button class="text-xs bg-transparent border border-purple-600 text-purple-600 hover:bg-purple-600 hover:text-white px-3 py-1.5 rounded-lg transition-colors duration-200">
                <i class="ri-check-line mr-1"></i>This was me
            </button>
        </div>
    </div>
    <button type="button" class="ml-4 -mx-1.5 -my-1.5 bg-purple-50 text-purple-500 rounded-lg focus:ring-2 focus:ring-purple-400 p-1.5 hover:bg-purple-200 inline-flex items-center justify-center h-8 w-8 dark:bg-gray-800 dark:text-purple-400 dark:hover:bg-gray-700 transition-colors duration-200" onclick="dismissAlert('security-alert')" aria-label="Close">
        <i class="ri-close-line text-lg"></i>
    </button>
</div>
```

## JavaScript Functions

Add these JavaScript functions for alert functionality:

```javascript
// Function to dismiss alerts
function dismissAlert(alertId) {
    const alert = document.getElementById(alertId);
    alert.style.transition = 'opacity 0.3s ease-out, transform 0.3s ease-out';
    alert.style.opacity = '0';
    alert.style.transform = 'translateX(100%)';
    setTimeout(() => {
        alert.style.display = 'none';
    }, 300);
}

// Function to show alert with animation
function showAlert(alertId) {
    const alert = document.getElementById(alertId);
    alert.style.display = 'flex';
    alert.style.opacity = '0';
    alert.style.transform = 'translateY(-20px)';
    setTimeout(() => {
        alert.style.transition = 'opacity 0.3s ease-out, transform 0.3s ease-out';
        alert.style.opacity = '1';
        alert.style.transform = 'translateY(0)';
    }, 10);
}
```
