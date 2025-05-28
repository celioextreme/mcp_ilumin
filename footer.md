# Footer Component Examples

## Example 1: Simple Footer with Social Links

```html
<footer class="bg-gray-800 text-white p-8">
    <div class="container mx-auto">
        <div class="flex flex-col md:flex-row justify-between items-center">
            <div class="mb-6 md:mb-0">
                <a href="#" class="text-2xl font-bold flex items-center">
                    <span class="bg-blue-500 text-white p-2 rounded-lg mr-2">
                        <i class="ri-code-box-line"></i>
                    </span>
                    Company Name
                </a>
            </div>
            <div class="flex space-x-6">
                <a href="#" class="hover:text-blue-400 transition-colors">
                    <i class="ri-facebook-circle-fill text-2xl"></i>
                </a>
                <a href="#" class="hover:text-blue-400 transition-colors">
                    <i class="ri-twitter-x-fill text-2xl"></i>
                </a>
                <a href="#" class="hover:text-blue-400 transition-colors">
                    <i class="ri-instagram-line text-2xl"></i>
                </a>
                <a href="#" class="hover:text-blue-400 transition-colors">
                    <i class="ri-linkedin-box-fill text-2xl"></i>
                </a>
                <a href="#" class="hover:text-blue-400 transition-colors">
                    <i class="ri-youtube-fill text-2xl"></i>
                </a>
            </div>
        </div>
        <div class="mt-8 border-t border-gray-700 pt-8 flex flex-col md:flex-row justify-between items-center">
            <p>© 2023 Company Name. All rights reserved.</p>
            <div class="mt-4 md:mt-0">
                <ul class="flex flex-wrap space-x-4">
                    <li><a href="#" class="hover:text-blue-400 transition-colors">Privacy Policy</a></li>
                    <li><a href="#" class="hover:text-blue-400 transition-colors">Terms of Service</a></li>
                    <li><a href="#" class="hover:text-blue-400 transition-colors">Contact Us</a></li>
                </ul>
            </div>
        </div>
    </div>
</footer>
```

## Example 2: Multi-Column Footer

```html
<footer class="bg-gray-900 text-gray-300 py-12">
    <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
            <!-- Column 1: About -->
            <div>
                <h3 class="text-lg font-semibold text-white mb-4">About Us</h3>
                <p class="mb-4">We create innovative solutions for businesses around the world, focusing on cutting-edge technologies that drive growth and success.</p>
                <div class="flex space-x-4">
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="ri-facebook-fill"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="ri-twitter-x-fill"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="ri-instagram-fill"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <i class="ri-linkedin-fill"></i>
                    </a>
                </div>
            </div>
            
            <!-- Column 2: Quick Links -->
            <div>
                <h3 class="text-lg font-semibold text-white mb-4">Quick Links</h3>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white transition-colors">Home</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">About Us</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Services</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Portfolio</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Testimonials</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Blog</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Contact</a></li>
                </ul>
            </div>
            
            <!-- Column 3: Services -->
            <div>
                <h3 class="text-lg font-semibold text-white mb-4">Our Services</h3>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white transition-colors">Web Development</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Mobile Applications</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">UI/UX Design</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Digital Marketing</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Cloud Solutions</a></li>
                    <li><a href="#" class="hover:text-white transition-colors">Consulting</a></li>
                </ul>
            </div>
            
            <!-- Column 4: Contact -->
            <div>
                <h3 class="text-lg font-semibold text-white mb-4">Contact Us</h3>
                <div class="space-y-3">
                    <p class="flex items-start">
                        <i class="ri-map-pin-line mr-3 mt-1"></i>
                        <span>1234 Street Name, City, Country</span>
                    </p>
                    <p class="flex items-start">
                        <i class="ri-phone-line mr-3 mt-1"></i>
                        <span>+1 (555) 123-4567</span>
                    </p>
                    <p class="flex items-start">
                        <i class="ri-mail-line mr-3 mt-1"></i>
                        <span>info@example.com</span>
                    </p>
                    <p class="flex items-start">
                        <i class="ri-time-line mr-3 mt-1"></i>
                        <span>Monday - Friday: 9:00 AM - 5:00 PM</span>
                    </p>
                </div>
            </div>
        </div>
        
        <div class="mt-12 pt-8 border-t border-gray-800 text-center">
            <p>© 2023 Company Name. All rights reserved.</p>
        </div>
    </div>
</footer>
```

## Example 3: Newsletter Subscription Footer

```html
<footer class="bg-indigo-900 text-white">
    <!-- Newsletter Section -->
    <div class="container mx-auto px-4 py-12">
        <div class="max-w-3xl mx-auto text-center">
            <h3 class="text-2xl font-bold mb-2">Subscribe to Our Newsletter</h3>
            <p class="text-indigo-200 mb-6">Stay updated with our latest news, updates and offers.</p>
            
            <form class="flex flex-col sm:flex-row gap-2">
                <input 
                    type="email" 
                    placeholder="Enter your email" 
                    class="flex-grow px-4 py-3 rounded-lg text-gray-800 focus:outline-none focus:ring-2 focus:ring-indigo-500"
                    required
                >
                <button 
                    type="submit" 
                    class="bg-indigo-500 hover:bg-indigo-600 px-6 py-3 rounded-lg font-semibold transition-colors duration-300 flex items-center justify-center"
                >
                    <i class="ri-send-plane-fill mr-2"></i> Subscribe
                </button>
            </form>
            <p class="text-xs text-indigo-300 mt-4">By subscribing, you agree to our Privacy Policy and consent to receive updates.</p>
        </div>
    </div>
    
    <!-- Main Footer -->
    <div class="border-t border-indigo-800">
        <div class="container mx-auto px-4 py-8">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <a href="#" class="text-2xl font-bold">
                        <span class="text-indigo-400">Company</span>Name
                    </a>
                </div>
                
                <div class="flex flex-wrap justify-center gap-x-6 gap-y-2 mb-6 md:mb-0">
                    <a href="#" class="hover:text-indigo-300 transition-colors">Home</a>
                    <a href="#" class="hover:text-indigo-300 transition-colors">About</a>
                    <a href="#" class="hover:text-indigo-300 transition-colors">Services</a>
                    <a href="#" class="hover:text-indigo-300 transition-colors">Projects</a>
                    <a href="#" class="hover:text-indigo-300 transition-colors">Contact</a>
                </div>
                
                <div class="flex space-x-4">
                    <a href="#" class="bg-indigo-800 hover:bg-indigo-700 w-9 h-9 rounded-full flex items-center justify-center transition-colors">
                        <i class="ri-facebook-fill"></i>
                    </a>
                    <a href="#" class="bg-indigo-800 hover:bg-indigo-700 w-9 h-9 rounded-full flex items-center justify-center transition-colors">
                        <i class="ri-twitter-x-fill"></i>
                    </a>
                    <a href="#" class="bg-indigo-800 hover:bg-indigo-700 w-9 h-9 rounded-full flex items-center justify-center transition-colors">
                        <i class="ri-instagram-line"></i>
                    </a>
                    <a href="#" class="bg-indigo-800 hover:bg-indigo-700 w-9 h-9 rounded-full flex items-center justify-center transition-colors">
                        <i class="ri-linkedin-fill"></i>
                    </a>
                </div>
            </div>
            
            <div class="mt-8 border-t border-indigo-800 pt-8 text-center text-indigo-300 text-sm">
                <p>© 2023 Company Name. All rights reserved.</p>
            </div>
        </div>
    </div>
</footer>
```

## Example 4: App Download Footer

```html
<footer class="bg-gradient-to-r from-blue-800 to-blue-600 text-white">
    <div class="container mx-auto px-4 py-12">
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <!-- Download App Section -->
            <div>
                <h3 class="text-2xl font-bold mb-4">Get Our Mobile App</h3>
                <p class="text-blue-100 mb-6">Download our app for a better experience on your mobile device. Access all features on the go!</p>
                <div class="flex flex-wrap gap-4">
                    <!-- App Store Button -->
                    <a href="#" class="bg-black hover:bg-gray-900 text-white px-4 py-3 rounded-lg flex items-center transition-colors">
                        <i class="ri-app-store-fill text-3xl mr-3"></i>
                        <div>
                            <div class="text-xs">Download on the</div>
                            <div class="text-xl font-semibold">App Store</div>
                        </div>
                    </a>
                    
                    <!-- Google Play Button -->
                    <a href="#" class="bg-black hover:bg-gray-900 text-white px-4 py-3 rounded-lg flex items-center transition-colors">
                        <i class="ri-google-play-fill text-3xl mr-3"></i>
                        <div>
                            <div class="text-xs">Get it on</div>
                            <div class="text-xl font-semibold">Google Play</div>
                        </div>
                    </a>
                </div>
            </div>
            
            <!-- Contact Info and Social Section -->
            <div class="grid sm:grid-cols-2 gap-8">
                <div>
                    <h4 class="font-bold text-lg mb-4">Contact Us</h4>
                    <div class="space-y-3 text-blue-100">
                        <p class="flex items-start">
                            <i class="ri-mail-line mr-3 mt-1"></i>
                            <span>support@example.com</span>
                        </p>
                        <p class="flex items-start">
                            <i class="ri-phone-line mr-3 mt-1"></i>
                            <span>+1 (555) 987-6543</span>
                        </p>
                        <p class="flex items-start">
                            <i class="ri-map-pin-line mr-3 mt-1"></i>
                            <span>123 App Street, Tech City, 10001</span>
                        </p>
                    </div>
                </div>
                
                <div>
                    <h4 class="font-bold text-lg mb-4">Follow Us</h4>
                    <div class="grid grid-cols-2 gap-4">
                        <a href="#" class="flex items-center text-blue-100 hover:text-white transition-colors">
                            <i class="ri-facebook-fill mr-2"></i> Facebook
                        </a>
                        <a href="#" class="flex items-center text-blue-100 hover:text-white transition-colors">
                            <i class="ri-twitter-x-fill mr-2"></i> Twitter
                        </a>
                        <a href="#" class="flex items-center text-blue-100 hover:text-white transition-colors">
                            <i class="ri-instagram-line mr-2"></i> Instagram
                        </a>
                        <a href="#" class="flex items-center text-blue-100 hover:text-white transition-colors">
                            <i class="ri-youtube-fill mr-2"></i> YouTube
                        </a>
                        <a href="#" class="flex items-center text-blue-100 hover:text-white transition-colors">
                            <i class="ri-linkedin-fill mr-2"></i> LinkedIn
                        </a>
                        <a href="#" class="flex items-center text-blue-100 hover:text-white transition-colors">
                            <i class="ri-pinterest-fill mr-2"></i> Pinterest
                        </a>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Copyright Section -->
        <div class="mt-12 pt-8 border-t border-blue-700">
            <div class="flex flex-col sm:flex-row justify-between items-center">
                <p class="mb-4 sm:mb-0">© 2023 App Name. All rights reserved.</p>
                <div class="flex space-x-4">
                    <a href="#" class="text-sm text-blue-100 hover:text-white transition-colors">Privacy Policy</a>
                    <a href="#" class="text-sm text-blue-100 hover:text-white transition-colors">Terms of Service</a>
                    <a href="#" class="text-sm text-blue-100 hover:text-white transition-colors">Cookie Policy</a>
                </div>
            </div>
        </div>
    </div>
</footer>
```

## Example 5: Sticky Footer with Back to Top Button

```html
<footer class="sticky bottom-0 w-full bg-emerald-800 text-white">
    <!-- Back to top button -->
    <div class="container mx-auto px-4 relative">
        <button onclick="window.scrollTo({top: 0, behavior: 'smooth'})" class="absolute -top-6 right-6 bg-emerald-500 text-white rounded-full w-12 h-12 flex items-center justify-center shadow-lg hover:bg-emerald-600 focus:outline-none focus:ring-2 focus:ring-emerald-400 transition-colors">
            <i class="ri-arrow-up-line text-xl"></i>
        </button>
    </div>
    
    <!-- Main footer content -->
    <div class="container mx-auto px-4 py-6">
        <div class="flex flex-col md:flex-row justify-between items-center">
            <div class="flex items-center mb-4 md:mb-0">
                <a href="#" class="text-xl font-bold mr-8">
                    <i class="ri-leaf-fill mr-2 text-emerald-400"></i> GreenTech
                </a>
                <nav>
                    <ul class="flex space-x-6 text-sm">
                        <li><a href="#" class="hover:text-emerald-300 transition-colors">Home</a></li>
                        <li><a href="#" class="hover:text-emerald-300 transition-colors">About</a></li>
                        <li><a href="#" class="hover:text-emerald-300 transition-colors">Features</a></li>
                        <li><a href="#" class="hover:text-emerald-300 transition-colors">Pricing</a></li>
                        <li><a href="#" class="hover:text-emerald-300 transition-colors">Contact</a></li>
                    </ul>
                </nav>
            </div>
            
            <div class="flex items-center space-x-4">
                <a href="#" class="text-emerald-200 hover:text-white transition-colors">
                    <i class="ri-facebook-fill"></i>
                </a>
                <a href="#" class="text-emerald-200 hover:text-white transition-colors">
                    <i class="ri-twitter-x-fill"></i>
                </a>
                <a href="#" class="text-emerald-200 hover:text-white transition-colors">
                    <i class="ri-instagram-line"></i>
                </a>
                <a href="#" class="text-emerald-200 hover:text-white transition-colors">
                    <i class="ri-github-fill"></i>
                </a>
            </div>
        </div>
        
        <div class="mt-4 pt-4 border-t border-emerald-700 flex flex-col sm:flex-row justify-between items-center text-emerald-200 text-sm">
            <p>© 2023 GreenTech. All rights reserved.</p>
            <div class="mt-2 sm:mt-0">
                <a href="#" class="hover:text-white transition-colors">Privacy</a>
                <span class="mx-2">•</span>
                <a href="#" class="hover:text-white transition-colors">Terms</a>
                <span class="mx-2">•</span>
                <a href="#" class="hover:text-white transition-colors">Cookies</a>
            </div>
        </div>
    </div>
</footer>
```
