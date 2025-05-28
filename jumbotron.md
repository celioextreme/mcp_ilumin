# Jumbotron Component Examples

## Example 1: Basic Jumbotron
```html
<div class="bg-gray-200 rounded-lg p-8 md:p-12">
    <h1 class="text-3xl md:text-4xl font-extrabold text-gray-900 mb-4">Welcome to Our Platform</h1>
    <p class="text-lg text-gray-700 mb-6">This is a simple jumbotron-style component for calling extra attention to featured content or information.</p>
    <button class="px-6 py-2 bg-blue-600 text-white font-medium rounded-md hover:bg-blue-700 transition duration-300">
        Learn more
    </button>
</div>
```

## Example 2: Jumbotron with Background Image
```html
<div class="relative rounded-lg overflow-hidden">
    <div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1522252234503-e356532cafd5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80');">
        <div class="absolute inset-0 bg-black opacity-60"></div>
    </div>
    <div class="relative z-10 p-8 md:p-12 lg:p-16">
        <h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-4">Develop with Confidence</h1>
        <p class="text-xl text-gray-200 mb-8 max-w-lg">Build beautiful, responsive websites with Tailwind CSS and take your development skills to the next level.</p>
        <div class="flex flex-col sm:flex-row gap-4">
            <button class="px-6 py-3 bg-white text-gray-900 font-medium rounded-md hover:bg-gray-100 transition duration-300">
                Get Started
            </button>
            <button class="px-6 py-3 bg-transparent border-2 border-white text-white font-medium rounded-md hover:bg-white/10 transition duration-300">
                View Demos
            </button>
        </div>
    </div>
</div>
```

## Example 3: Jumbotron with Cards
```html
<div class="bg-gradient-to-r from-blue-600 to-indigo-700 rounded-lg p-8 md:p-10">
    <div class="max-w-4xl mx-auto">
        <h1 class="text-3xl md:text-4xl font-bold text-white mb-3 text-center">Our Services</h1>
        <p class="text-lg text-blue-100 mb-8 text-center">Choose the perfect plan for your business needs</p>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <!-- Card 1 -->
            <div class="bg-white rounded-lg shadow-md overflow-hidden transition transform hover:-translate-y-1 hover:shadow-lg">
                <div class="p-6">
                    <div class="flex justify-center mb-4">
                        <div class="w-14 h-14 bg-blue-100 rounded-full flex items-center justify-center">
                            <i class="ri-rocket-line text-2xl text-blue-600"></i>
                        </div>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-2 text-center">Starter</h3>
                    <p class="text-center text-gray-600 mb-6">Perfect for small projects</p>
                    <div class="text-center mb-6">
                        <span class="text-4xl font-bold text-gray-800">$19</span>
                        <span class="text-gray-600">/month</span>
                    </div>
                    <button class="w-full py-2 bg-blue-600 text-white rounded-md hover:bg-blue-700 transition duration-300">
                        Get Started
                    </button>
                </div>
            </div>
            <!-- More cards -->
        </div>
    </div>
</div>
```

## Example 4: Jumbotron with Video Background
```html
<div class="relative rounded-lg overflow-hidden h-96">
    <!-- Video element would typically go here -->
    <div class="absolute inset-0 bg-gray-900">
        <div class="w-full h-full flex items-center justify-center text-white">
            <div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1531297484001-80022131f5a1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80');">
                <div class="absolute inset-0 bg-black opacity-70"></div>
            </div>
            <!-- Play button overlay -->
            <button class="relative z-10 w-20 h-20 bg-white/20 rounded-full flex items-center justify-center backdrop-blur-sm hover:bg-white/30 transition duration-300 group">
                <div class="w-16 h-16 bg-white rounded-full flex items-center justify-center">
                    <i class="ri-play-fill text-3xl text-blue-600 group-hover:scale-110 transition duration-300"></i>
                </div>
            </button>
        </div>
    </div>
    <div class="absolute bottom-0 left-0 right-0 p-8 z-10">
        <h1 class="text-3xl font-bold text-white mb-2">Watch Our Story</h1>
        <p class="text-lg text-white/80">Learn how we're changing the way people connect with technology.</p>
    </div>
</div>
```

## Example 5: Animated Jumbotron with Particles
```html
<div class="relative rounded-lg overflow-hidden h-96 bg-gradient-to-br from-violet-600 to-indigo-800">
    <!-- Particle dots (static, but would be animated with JS in real implementation) -->
    <div class="absolute inset-0 overflow-hidden">
        <div class="particles">
            <!-- These static dots simulate the particles -->
            <div class="absolute w-3 h-3 rounded-full bg-white/10" style="top: 10%; left: 20%"></div>
            <div class="absolute w-2 h-2 rounded-full bg-white/20" style="top: 30%; left: 70%"></div>
            <!-- More particles -->
        </div>
    </div>
    
    <!-- Content -->
    <div class="relative z-10 flex items-center justify-center h-full">
        <div class="text-center px-6">
            <div class="inline-block p-2 rounded-lg bg-white/10 backdrop-blur-sm mb-6">
                <span class="text-white text-sm font-medium px-3 py-1">New Release</span>
            </div>
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">Introducing Our <span class="text-transparent bg-clip-text bg-gradient-to-r from-yellow-400 to-pink-400">Next-Gen</span> Platform</h1>
            <p class="text-xl text-indigo-100 mb-8 max-w-2xl mx-auto">Experience the future of web development with our innovative tools and frameworks.</p>
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <button class="px-8 py-3 bg-white text-indigo-700 font-medium rounded-full hover:bg-gray-100 transition duration-300 flex items-center">
                    <i class="ri-download-line mr-2"></i>
                    Download Now
                </button>
                <button class="px-8 py-3 bg-transparent border-2 border-white/50 text-white font-medium rounded-full hover:border-white transition duration-300 flex items-center">
                    <i class="ri-play-circle-line mr-2"></i>
                    Watch Demo
                </button>
            </div>
        </div>
    </div>
</div>
```
