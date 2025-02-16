### **Login Page Structure (Mobile-First Layout)**  

1. **Header**  
   - Logo / App Name (Centered or Left-Aligned)  
   - Optional Back Button (to return to Home)  

2. **Main Content (Centered Login Form)**  
   - **Page Title:** "Login to Your Account" (Large & Bold)  
   - **Input Fields:**  
     - Email Input Field  
     - Password Input Field  
   - **Action Button:**  
     - "Login" Button (Primary, Full Width)  
   - **Alternative Options:**  
     - "Forgot Password?" (Small, Link Below Password)  
     - "Don't have an account? Sign Up" (Secondary Link)  

3. **Optional Social Login Section** (Below Form)  
   - "Or Sign in with" (Small Text)  
   - Social Media Login Buttons (Google, Facebook, etc.)  

4. **Footer (Minimalist)**  
   - Terms of Service & Privacy Policy Links (Small, Centered)  

---

### 🎨 Prototype

```vue
<template>
  <div class="min-h-screen flex flex-col justify-center items-center bg-gray-100 dark:bg-gray-900 text-gray-900 dark:text-white px-6">
    <!-- Header -->
    <header class="absolute top-4 left-4 text-xl font-bold">
      <NuxtLink to="/" class="hover:text-blue-500">SBP</NuxtLink>
    </header>

    <!-- Login Form -->
    <div class="w-full max-w-md p-6 bg-white dark:bg-gray-800 shadow-md rounded-lg">
      <h2 class="text-2xl font-bold text-center">Login to Your Account</h2>
      
      <form class="mt-6 space-y-4">
        <div>
          <label class="block text-sm font-medium">Email</label>
          <input type="email" class="w-full px-4 py-2 mt-1 border rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" required />
        </div>
        
        <div>
          <label class="block text-sm font-medium">Password</label>
          <input type="password" class="w-full px-4 py-2 mt-1 border rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" required />
        </div>
        
        <NuxtLink to="/forgot-password" class="text-sm text-blue-500 hover:underline">Forgot Password?</NuxtLink>
        
        <button type="submit" class="w-full bg-blue-500 text-white py-2 rounded-md hover:bg-blue-600">Login</button>
      </form>

      <!-- Sign Up Link -->
      <p class="mt-4 text-center text-sm">
        Don't have an account? 
        <NuxtLink to="/signup" class="text-blue-500 hover:underline">Sign Up</NuxtLink>
      </p>
    </div>

    <!-- Footer -->
    <footer class="mt-6 text-xs text-gray-500 dark:text-gray-400">
      <NuxtLink to="/terms" class="hover:underline">Terms of Service</NuxtLink> • 
      <NuxtLink to="/privacy" class="hover:underline">Privacy Policy</NuxtLink>
    </footer>
  </div>
</template>
```

**Nuxt 3 + Tailwind CSS** login 

It includes:  
✅ **Mobile-first responsive design**  
✅ **Dark mode support**  
✅ **Form validation-ready structure**  
✅ **Links to "Forgot Password" and "Sign Up"**  

Let me know if you need further refinements! 
