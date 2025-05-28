# Modal Components - Individual Codes

## Example 1: Confirmation Modal
Use for delete confirmations and destructive actions.

```html
<!-- Trigger Button -->
<a href="#confirmationModal" class="bg-red-600 text-white px-4 py-2 rounded-lg hover:bg-red-700 transition-colors duration-200 inline-block text-center">
    Open Confirmation Modal
</a>

<!-- Modal -->
<div id="confirmationModal" class="modal fixed inset-0 z-50 flex items-center justify-center opacity-0 visibility-hidden backdrop-blur-sm bg-black bg-opacity-50 transition-all duration-300">
    <div class="modal-content bg-white rounded-2xl p-8 max-w-md mx-4 shadow-2xl transform scale-90 transition-transform duration-300">
        <div class="text-center">
            <div class="w-20 h-20 bg-red-100 rounded-full flex items-center justify-center mx-auto mb-6">
                <i class="ri-delete-bin-line text-3xl text-red-600"></i>
            </div>
            <h3 class="text-2xl font-bold text-gray-900 mb-4">Delete Item</h3>
            <p class="text-gray-600 mb-8 leading-relaxed">
                Are you sure you want to delete this item? This action cannot be undone and will permanently remove the data from our servers.
            </p>
            <div class="flex space-x-4">
                <a href="#" class="flex-1 bg-gray-100 text-gray-700 px-6 py-3 rounded-xl hover:bg-gray-200 transition-colors duration-200 font-medium text-center">
                    Cancel
                </a>
                <a href="#" class="flex-1 bg-red-600 text-white px-6 py-3 rounded-xl hover:bg-red-700 transition-colors duration-200 font-medium text-center">
                    Delete
                </a>
            </div>
        </div>
    </div>
</div>
```

## Example 2: Success Modal
Use for showing success messages and confirmations.

```html
<!-- Trigger Button -->
<a href="#successModal" class="bg-green-600 text-white px-4 py-2 rounded-lg hover:bg-green-700 transition-colors duration-200 inline-block text-center">
    Open Success Modal
</a>

<!-- Modal -->
<div id="successModal" class="modal fixed inset-0 z-50 flex items-center justify-center opacity-0 visibility-hidden backdrop-blur-sm bg-black bg-opacity-50 transition-all duration-300">
    <div class="modal-content bg-white rounded-2xl p-8 max-w-md mx-4 shadow-2xl transform scale-90 transition-transform duration-300">
        <div class="text-center">
            <div class="w-20 h-20 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-6">
                <i class="ri-checkbox-circle-line text-3xl text-green-600"></i>
            </div>
            <h3 class="text-2xl font-bold text-gray-900 mb-4">Success!</h3>
            <p class="text-gray-600 mb-8 leading-relaxed">
                Your action has been completed successfully. Thank you for using our service!
            </p>
            <div class="bg-green-50 border border-green-200 rounded-xl p-4 mb-6">
                <div class="flex items-center text-green-800">
                    <i class="ri-information-line text-lg mr-2"></i>
                    <span class="text-sm font-medium">You will receive a confirmation email shortly.</span>
                </div>
            </div>
            <a href="#" class="w-full bg-green-600 text-white px-6 py-3 rounded-xl hover:bg-green-700 transition-colors duration-200 font-medium inline-block text-center">
                Continue
            </a>
        </div>
    </div>
</div>
```

## Example 3: Profile Modal
Use for user profile editing and form inputs.

```html
<!-- Trigger Button -->
<a href="#profileModal" class="bg-blue-600 text-white px-4 py-2 rounded-lg hover:bg-blue-700 transition-colors duration-200 inline-block text-center">
    Open Profile Modal
</a>

<!-- Modal -->
<div id="profileModal" class="modal fixed inset-0 z-50 flex items-center justify-center opacity-0 visibility-hidden backdrop-blur-sm bg-black bg-opacity-50 transition-all duration-300">
    <div class="modal-content bg-white rounded-2xl p-8 max-w-lg mx-4 shadow-2xl transform scale-90 transition-transform duration-300">
        <div class="flex items-center justify-between mb-6">
            <h3 class="text-2xl font-bold text-gray-900">Edit Profile</h3>
            <a href="#" class="text-gray-400 hover:text-gray-600 transition-colors duration-200">
                <i class="ri-close-line text-2xl"></i>
            </a>
        </div>
        
        <div class="space-y-6">
            <div class="flex justify-center mb-6">
                <div class="relative">
                    <div class="w-24 h-24 bg-blue-100 rounded-full flex items-center justify-center">
                        <i class="ri-user-line text-3xl text-blue-600"></i>
                    </div>
                    <div class="absolute -bottom-2 -right-2 w-8 h-8 bg-blue-600 text-white rounded-full flex items-center justify-center hover:bg-blue-700 transition-colors duration-200 cursor-pointer">
                        <i class="ri-camera-line text-sm"></i>
                    </div>
                </div>
            </div>
            
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-2">Full Name</label>
                <input type="text" value="John Doe" class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-200">
            </div>
            
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-2">Email</label>
                <input type="email" value="john@example.com" class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-200">
            </div>
            
            <div>
                <label class="block text-sm font-medium text-gray-700 mb-2">Bio</label>
                <textarea rows="3" class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-200" placeholder="Tell us about yourself..."></textarea>
            </div>
        </div>
        
        <div class="flex space-x-4 mt-8">
            <a href="#" class="flex-1 bg-gray-100 text-gray-700 px-6 py-3 rounded-xl hover:bg-gray-200 transition-colors duration-200 font-medium text-center">
                Cancel
            </a>
            <a href="#" class="flex-1 bg-blue-600 text-white px-6 py-3 rounded-xl hover:bg-blue-700 transition-colors duration-200 font-medium text-center">
                Save Changes
            </a>
        </div>
    </div>
</div>
```

## Example 4: Notification Settings Modal
Use for settings and preferences with toggle options.

```html
<!-- Trigger Button -->
<a href="#notificationModal" class="bg-purple-600 text-white px-4 py-2 rounded-lg hover:bg-purple-700 transition-colors duration-200 inline-block text-center">
    Open Settings Modal
</a>

<!-- Modal -->
<div id="notificationModal" class="modal fixed inset-0 z-50 flex items-center justify-center opacity-0 visibility-hidden backdrop-blur-sm bg-black bg-opacity-50 transition-all duration-300">
    <div class="modal-content bg-white rounded-2xl p-8 max-w-md mx-4 shadow-2xl transform scale-90 transition-transform duration-300">
        <div class="flex items-center justify-between mb-6">
            <h3 class="text-2xl font-bold text-gray-900">Notification Settings</h3>
            <a href="#" class="text-gray-400 hover:text-gray-600 transition-colors duration-200">
                <i class="ri-close-line text-2xl"></i>
            </a>
        </div>
        
        <div class="space-y-6">
            <div class="flex items-center justify-between p-4 bg-purple-50 rounded-xl">
                <div class="flex items-center">
                    <i class="ri-mail-line text-purple-600 text-xl mr-3"></i>
                    <div>
                        <h4 class="font-medium text-gray-900">Email Notifications</h4>
                        <p class="text-sm text-gray-600">Receive updates via email</p>
                    </div>
                </div>
                <label class="relative inline-flex items-center cursor-pointer">
                    <input type="checkbox" checked class="toggle-switch relative w-11 h-6 rounded-full appearance-none cursor-pointer bg-purple-600">
                </label>
            </div>
            
            <div class="flex items-center justify-between p-4 bg-purple-50 rounded-xl">
                <div class="flex items-center">
                    <i class="ri-smartphone-line text-purple-600 text-xl mr-3"></i>
                    <div>
                        <h4 class="font-medium text-gray-900">Push Notifications</h4>
                        <p class="text-sm text-gray-600">Receive push notifications</p>
                    </div>
                </div>
                <label class="relative inline-flex items-center cursor-pointer">
                    <input type="checkbox" class="toggle-switch relative w-11 h-6 rounded-full appearance-none cursor-pointer bg-gray-300">
                </label>
            </div>
            
            <div class="flex items-center justify-between p-4 bg-purple-50 rounded-xl">
                <div class="flex items-center">
                    <i class="ri-calendar-line text-purple-600 text-xl mr-3"></i>
                    <div>
                        <h4 class="font-medium text-gray-900">Calendar Reminders</h4>
                        <p class="text-sm text-gray-600">Get reminded about events</p>
                    </div>
                </div>
                <label class="relative inline-flex items-center cursor-pointer">
                    <input type="checkbox" checked class="toggle-switch relative w-11 h-6 rounded-full appearance-none cursor-pointer bg-purple-600">
                </label>
            </div>
        </div>
        
        <a href="#" class="w-full bg-purple-600 text-white px-6 py-3 rounded-xl hover:bg-purple-700 transition-colors duration-200 font-medium mt-8 inline-block text-center">
            Save Settings
        </a>
    </div>
</div>
```

## Example 5: Image Gallery Modal
Use for displaying images with navigation and actions.

```html
<!-- Trigger Button -->
<a href="#galleryModal" class="bg-orange-600 text-white px-4 py-2 rounded-lg hover:bg-orange-700 transition-colors duration-200 inline-block text-center">
    Open Gallery Modal
</a>

<!-- Modal -->
<div id="galleryModal" class="modal fixed inset-0 z-50 flex items-center justify-center opacity-0 visibility-hidden backdrop-blur-sm bg-black bg-opacity-50 transition-all duration-300">
    <div class="modal-content bg-white rounded-2xl p-8 max-w-2xl mx-4 shadow-2xl transform scale-90 transition-transform duration-300">
        <div class="flex items-center justify-between mb-6">
            <h3 class="text-2xl font-bold text-gray-900">Image Gallery</h3>
            <a href="#" class="text-gray-400 hover:text-gray-600 transition-colors duration-200">
                <i class="ri-close-line text-2xl"></i>
            </a>
        </div>
        
        <div class="space-y-6">
            <!-- Main Image Display -->
            <div class="relative bg-gray-100 rounded-xl h-64 flex items-center justify-center">
                <div class="text-center">
                    <i class="ri-image-line text-6xl text-gray-400 mb-4"></i>
                    <p class="text-gray-600 font-medium">Sample Image Preview</p>
                    <p class="text-sm text-gray-500">1920 x 1080 pixels</p>
                </div>
                
                <!-- Navigation Arrows -->
                <div class="absolute left-4 top-1/2 transform -translate-y-1/2 w-10 h-10 bg-white rounded-full shadow-lg flex items-center justify-center hover:bg-gray-50 transition-colors duration-200 cursor-pointer">
                    <i class="ri-arrow-left-line text-gray-600"></i>
                </div>
                <div class="absolute right-4 top-1/2 transform -translate-y-1/2 w-10 h-10 bg-white rounded-full shadow-lg flex items-center justify-center hover:bg-gray-50 transition-colors duration-200 cursor-pointer">
                    <i class="ri-arrow-right-line text-gray-600"></i>
                </div>
            </div>
            
            <!-- Thumbnail Gallery -->
            <div class="grid grid-cols-4 gap-3">
                <div class="bg-orange-100 rounded-lg h-16 flex items-center justify-center border-2 border-orange-500">
                    <i class="ri-image-line text-orange-600"></i>
                </div>
                <div class="bg-gray-100 rounded-lg h-16 flex items-center justify-center border-2 border-transparent hover:border-orange-300 cursor-pointer transition-colors duration-200">
                    <i class="ri-image-line text-gray-400"></i>
                </div>
                <div class="bg-gray-100 rounded-lg h-16 flex items-center justify-center border-2 border-transparent hover:border-orange-300 cursor-pointer transition-colors duration-200">
                    <i class="ri-image-line text-gray-400"></i>
                </div>
                <div class="bg-gray-100 rounded-lg h-16 flex items-center justify-center border-2 border-transparent hover:border-orange-300 cursor-pointer transition-colors duration-200">
                    <i class="ri-image-line text-gray-400"></i>
                </div>
            </div>
            
            <!-- Image Info -->
            <div class="bg-orange-50 rounded-xl p-4">
                <div class="flex items-center justify-between">
                    <div>
                        <h4 class="font-medium text-gray-900">Beautiful Landscape</h4>
                        <p class="text-sm text-gray-600">Image 1 of 4</p>
                    </div>
                    <div class="flex space-x-2">
                        <div class="w-8 h-8 bg-orange-100 rounded-lg flex items-center justify-center hover:bg-orange-200 transition-colors duration-200 cursor-pointer">
                            <i class="ri-download-line text-orange-600"></i>
                        </div>
                        <div class="w-8 h-8 bg-orange-100 rounded-lg flex items-center justify-center hover:bg-orange-200 transition-colors duration-200 cursor-pointer">
                            <i class="ri-share-line text-orange-600"></i>
                        </div>
                        <div class="w-8 h-8 bg-orange-100 rounded-lg flex items-center justify-center hover:bg-orange-200 transition-colors duration-200 cursor-pointer">
                            <i class="ri-heart-line text-orange-600"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- CSS for modal functionality -->
<style>
.modal {
    opacity: 0;
    visibility: hidden;
    transform: scale(0.9) translateY(-20px);
    transition: all 0.3s ease;
    backdrop-filter: blur(4px);
    background-color: rgba(0, 0, 0, 0.5);
}

.modal:target {
    opacity: 1;
    visibility: visible;
    transform: scale(1) translateY(0);
}

.modal-content {
    transform: scale(0.9);
    transition: transform 0.3s ease;
}

.modal:target .modal-content {
    transform: scale(1);
}

.toggle-switch {
    background-color: #e5e7eb;
    transition: background-color 0.3s ease;
}

.toggle-switch:checked {
    background-color: #8b5cf6;
}

.toggle-switch::after {
    content: '';
    position: absolute;
    top: 2px;
    left: 2px;
    width: 20px;
    height: 20px;
    background-color: white;
    border-radius: 50%;
    transition: transform 0.3s ease;
}

.toggle-switch:checked::after {
    transform: translateX(20px);
}
</style>
```

## CSS Dependencies
Remember to include Tailwind CSS and Remix Icons:

```html
<script src="https://cdn.tailwindcss.com"></script>
<link href="https://cdn.jsdelivr.net/npm/remixicon@4.3.0/fonts/remixicon.css" rel="stylesheet">
```
