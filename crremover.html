<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Video Optimizer – Privacy Cleaner for Videos | Metadata Remover & Compressor</title>
    <meta name="description" content="Remove metadata, compress and optimize videos directly in your browser. 100% private.">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#eef2ff', 100: '#e0e7ff', 200: '#c7d2fe', 300: '#a5b4fc',
                            400: '#818cf8', 500: '#6366f1', 600: '#4f46e5', 700: '#4338ca',
                            800: '#3730a3', 900: '#312e81'
                        }
                    }
                }
            }
        }
    </script>
    <style>
        * { box-sizing: border-box; }
        html { scroll-behavior: smooth; }
        body { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; }
        
        .fade-in { animation: fadeIn 0.5s ease-out; }
        .slide-up { animation: slideUp 0.5s ease-out; }
        .slide-down { animation: slideDown 0.4s ease-out; }
        
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes slideUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes slideDown { from { opacity: 0; transform: translateY(-10px); } to { opacity: 1; transform: translateY(0); } }
        
        .drag-active { border-color: #6366f1 !important; background-color: rgba(99, 102, 241, 0.05) !important; }
        .dark .drag-active { background-color: rgba(99, 102, 241, 0.15) !important; }
        
        /* Toggle Switch */
        .toggle-track { width: 44px; height: 24px; border-radius: 12px; background: #d1d5db; transition: background 0.3s; position: relative; cursor: pointer; flex-shrink: 0; }
        .toggle-track.active { background: #6366f1; }
        .toggle-thumb { width: 20px; height: 20px; border-radius: 50%; background: white; position: absolute; top: 2px; left: 2px; transition: transform 0.3s; box-shadow: 0 1px 3px rgba(0,0,0,0.2); }
        .toggle-track.active .toggle-thumb { transform: translateX(20px); }
        .dark .toggle-track { background: #4b5563; }
        .dark .toggle-track.active { background: #6366f1; }
        
        /* Level Button */
        .level-btn { transition: all 0.2s; }
        .level-btn.selected { background: #eef2ff; border-color: #818cf8; color: #4338ca; }
        .dark .level-btn.selected { background: rgba(99,102,241,0.15); border-color: rgba(129,140,248,0.5); color: #a5b4fc; }
        
        /* Progress Bar */
        .progress-fill {
            background: linear-gradient(90deg, #6366f1, #818cf8, #6366f1);
            background-size: 200% 100%;
            animation: shimmer 2s linear infinite;
            transition: width 0.3s ease-out;
        }
        @keyframes shimmer { 0% { background-position: -200% 0; } 100% { background-position: 200% 0; } }
        
        /* Scrollbar */
        .log-container::-webkit-scrollbar { width: 4px; }
        .log-container::-webkit-scrollbar-track { background: transparent; }
        .log-container::-webkit-scrollbar-thumb { background: #9ca3af; border-radius: 2px; }
        .dark .log-container::-webkit-scrollbar-thumb { background: #4b5563; }
        
        ::selection { background: rgba(99,102,241,0.3); }
    </style>
</head>
<body class="bg-gray-50 dark:bg-gray-950 text-gray-900 dark:text-gray-100 min-h-screen transition-colors duration-300">

<!-- NAVBAR -->
<nav class="fixed top-0 left-0 right-0 z-50 bg-white/80 dark:bg-gray-900/80 backdrop-blur-xl border-b border-gray-200 dark:border-gray-800 transition-colors duration-300">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 h-16 flex items-center justify-between">
        <div class="flex items-center space-x-3">
            <div class="w-9 h-9 bg-gradient-to-br from-brand-500 to-brand-700 rounded-lg flex items-center justify-center shadow-lg">
                <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
            </div>
            <span class="text-xl font-bold bg-gradient-to-r from-brand-600 to-brand-400 bg-clip-text text-transparent">Video Optimizer</span>
        </div>
        <div class="flex items-center space-x-3">
            <span id="engineBadge" class="hidden sm:flex items-center px-3 py-1.5 rounded-full text-xs font-medium bg-yellow-100 dark:bg-yellow-900/30 text-yellow-700 dark:text-yellow-400">
                <span class="w-2 h-2 rounded-full bg-yellow-500 animate-pulse mr-2"></span>
                <span id="engineBadgeText">Loading...</span>
            </span>
            <button id="themeBtn" class="p-2.5 rounded-xl bg-gray-100 dark:bg-gray-800 hover:bg-gray-200 dark:hover:bg-gray-700 transition-colors" aria-label="Toggle theme">
                <svg id="sunIcon" class="w-5 h-5 text-yellow-500 block dark:hidden" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"/></svg>
                <svg id="moonIcon" class="w-5 h-5 text-brand-400 hidden dark:block" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"/></svg>
            </button>
        </div>
    </div>
</nav>

<!-- HERO -->
<section class="pt-24 pb-12 relative overflow-hidden">
    <div class="absolute inset-0 bg-gradient-to-br from-brand-50 via-white to-indigo-50 dark:from-gray-950 dark:via-gray-900 dark:to-indigo-950/30"></div>
    <div class="relative max-w-4xl mx-auto px-4 sm:px-6 text-center fade-in">
        <div class="inline-flex items-center px-4 py-2 rounded-full text-sm font-semibold bg-brand-100 dark:bg-brand-900/30 text-brand-700 dark:text-brand-300 mb-6">
            <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"/></svg>
            100% Client-Side Processing
        </div>
        <h1 class="text-5xl sm:text-6xl font-extrabold tracking-tight">
            <span class="bg-gradient-to-r from-gray-900 via-brand-800 to-gray-900 dark:from-white dark:via-brand-300 dark:to-white bg-clip-text text-transparent">Video Optimizer</span>
        </h1>
        <p class="mt-6 text-xl text-gray-600 dark:text-gray-300 max-w-2xl mx-auto">
            Privacy Cleaner for Videos – Remove Metadata &amp; Compress Files Instantly
        </p>
        <div class="mt-10 grid grid-cols-1 sm:grid-cols-2 gap-3 max-w-xl mx-auto text-left">
            <div class="flex items-center space-x-3 px-4 py-3 rounded-xl bg-white/60 dark:bg-gray-800/60 backdrop-blur-sm border border-gray-200/50 dark:border-gray-700/50">
                <div class="w-8 h-8 rounded-lg bg-green-100 dark:bg-green-900/30 flex items-center justify-center flex-shrink-0">
                    <svg class="w-4 h-4 text-green-600 dark:text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
                </div>
                <span class="text-sm font-medium text-gray-700 dark:text-gray-300">100% Private – Runs in Your Browser</span>
            </div>
            <div class="flex items-center space-x-3 px-4 py-3 rounded-xl bg-white/60 dark:bg-gray-800/60 backdrop-blur-sm border border-gray-200/50 dark:border-gray-700/50">
                <div class="w-8 h-8 rounded-lg bg-blue-100 dark:bg-blue-900/30 flex items-center justify-center flex-shrink-0">
                    <svg class="w-4 h-4 text-blue-600 dark:text-blue-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
                </div>
                <span class="text-sm font-medium text-gray-700 dark:text-gray-300">No Upload Required</span>
            </div>
            <div class="flex items-center space-x-3 px-4 py-3 rounded-xl bg-white/60 dark:bg-gray-800/60 backdrop-blur-sm border border-gray-200/50 dark:border-gray-700/50">
                <div class="w-8 h-8 rounded-lg bg-purple-100 dark:bg-purple-900/30 flex items-center justify-center flex-shrink-0">
                    <svg class="w-4 h-4 text-purple-600 dark:text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
                </div>
                <span class="text-sm font-medium text-gray-700 dark:text-gray-300">Fast Compression with Minimal Quality Loss</span>
            </div>
            <div class="flex items-center space-x-3 px-4 py-3 rounded-xl bg-white/60 dark:bg-gray-800/60 backdrop-blur-sm border border-gray-200/50 dark:border-gray-700/50">
                <div class="w-8 h-8 rounded-lg bg-orange-100 dark:bg-orange-900/30 flex items-center justify-center flex-shrink-0">
                    <svg class="w-4 h-4 text-orange-600 dark:text-orange-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
                </div>
                <span class="text-sm font-medium text-gray-700 dark:text-gray-300">One-Click Metadata Removal</span>
            </div>
        </div>
        <div class="mt-10">
            <button id="heroUploadBtn" class="inline-flex items-center px-8 py-4 text-lg font-semibold text-white bg-gradient-to-r from-brand-600 to-brand-500 hover:from-brand-700 hover:to-brand-600 rounded-2xl shadow-xl shadow-brand-500/25 hover:shadow-brand-500/40 transition-all duration-300 transform hover:scale-[1.02] active:scale-[0.98]">
                <svg class="w-6 h-6 mr-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"/></svg>
                Upload Video
            </button>
            <p class="mt-3 text-sm text-gray-500 dark:text-gray-400">Supports MP4, MOV, AVI, MKV • Max 2GB</p>
        </div>
    </div>
</section>

<!-- APP SECTION -->
<section class="max-w-4xl mx-auto px-4 sm:px-6 pb-20" id="appArea">

    <!-- DROP ZONE -->
    <div id="dropZone" class="bg-white dark:bg-gray-900 rounded-3xl border-2 border-dashed border-gray-300 dark:border-gray-700 hover:border-brand-400 dark:hover:border-brand-500 transition-all duration-300 p-12 text-center cursor-pointer group relative">
        <input type="file" id="fileInput" class="hidden" accept=".mp4,.mov,.avi,.mkv,video/mp4,video/quicktime,video/x-msvideo,video/x-matroska">
        <div class="space-y-4">
            <div class="mx-auto w-20 h-20 rounded-2xl bg-brand-50 dark:bg-brand-900/20 flex items-center justify-center group-hover:scale-110 transition-transform duration-300">
                <svg class="w-10 h-10 text-brand-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"/></svg>
            </div>
            <p class="text-xl font-semibold text-gray-700 dark:text-gray-200">Drop your video here</p>
            <p class="text-sm text-gray-500 dark:text-gray-400">or <span class="text-brand-600 dark:text-brand-400 font-medium">browse files</span></p>
            <p class="text-xs text-gray-400 dark:text-gray-500">MP4, MOV, AVI, MKV • Up to 2GB</p>
        </div>
    </div>

    <!-- FILE INFO + OPTIONS PANEL -->
    <div id="filePanel" class="hidden mt-6 slide-up">
        <div class="bg-white dark:bg-gray-900 rounded-3xl shadow-xl border border-gray-100 dark:border-gray-800 overflow-hidden">
            
            <!-- File Header -->
            <div class="p-6 border-b border-gray-100 dark:border-gray-800">
                <div class="flex items-center justify-between">
                    <div class="flex items-center space-x-4 min-w-0">
                        <div class="w-12 h-12 rounded-xl bg-brand-100 dark:bg-brand-900/30 flex items-center justify-center flex-shrink-0">
                            <svg class="w-6 h-6 text-brand-600 dark:text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
                        </div>
                        <div class="min-w-0">
                            <h3 id="dispFileName" class="font-semibold text-gray-900 dark:text-white truncate"></h3>
                            <div class="flex flex-wrap items-center gap-x-3 gap-y-1 mt-1 text-sm text-gray-500 dark:text-gray-400">
                                <span id="dispFileSize"></span>
                                <span>•</span>
                                <span id="dispDuration"></span>
                                <span>•</span>
                                <span id="dispFormat"></span>
                            </div>
                        </div>
                    </div>
                    <button id="removeFileBtn" class="p-2 rounded-xl hover:bg-red-50 dark:hover:bg-red-900/20 text-gray-400 hover:text-red-500 transition-colors flex-shrink-0 ml-2" aria-label="Remove file">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/></svg>
                    </button>
                </div>
            </div>

            <!-- Video Preview -->
            <div class="px-6 pt-4">
                <video id="videoPreview" class="w-full max-h-56 rounded-xl bg-black object-contain" controls preload="metadata"></video>
            </div>

            <!-- Options -->
            <div class="p-6 space-y-5">
                <h4 class="text-lg font-semibold text-gray-900 dark:text-white flex items-center">
                    <svg class="w-5 h-5 mr-2 text-brand-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.066 2.573c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.573 1.066c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.066-2.573c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"/><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                    Processing Options
                </h4>

                <!-- Toggle: Remove Metadata -->
                <div class="flex items-center justify-between p-4 rounded-2xl bg-gray-50 dark:bg-gray-800/50 hover:bg-gray-100 dark:hover:bg-gray-800 transition-colors cursor-pointer" id="metadataToggleRow">
                    <div class="flex items-center space-x-3">
                        <div class="w-10 h-10 rounded-xl bg-red-100 dark:bg-red-900/30 flex items-center justify-center flex-shrink-0">
                            <svg class="w-5 h-5 text-red-600 dark:text-red-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/></svg>
                        </div>
                        <div>
                            <p class="font-medium text-gray-900 dark:text-white">Remove Metadata Only</p>
                            <p class="text-sm text-gray-500 dark:text-gray-400">Strip all personal data & GPS info</p>
                        </div>
                    </div>
                    <div id="metadataToggle" class="toggle-track active"><div class="toggle-thumb"></div></div>
                </div>

                <!-- Toggle: Compress -->
                <div class="flex items-center justify-between p-4 rounded-2xl bg-gray-50 dark:bg-gray-800/50 hover:bg-gray-100 dark:hover:bg-gray-800 transition-colors cursor-pointer" id="compressToggleRow">
                    <div class="flex items-center space-x-3">
                        <div class="w-10 h-10 rounded-xl bg-blue-100 dark:bg-blue-900/30 flex items-center justify-center flex-shrink-0">
                            <svg class="w-5 h-5 text-blue-600 dark:text-blue-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"/></svg>
                        </div>
                        <div>
                            <p class="font-medium text-gray-900 dark:text-white">Optimize & Compress Video</p>
                            <p class="text-sm text-gray-500 dark:text-gray-400">Re-encode for smaller file size</p>
                        </div>
                    </div>
                    <div id="compressToggle" class="toggle-track"><div class="toggle-thumb"></div></div>
                </div>

                <!-- Compression Options -->
                <div id="compressOptions" class="hidden space-y-4 slide-down">
                    <div class="p-4 rounded-2xl bg-gray-50 dark:bg-gray-800/50">
                        <p class="font-medium text-gray-900 dark:text-white mb-3">Compression Level</p>
                        <div class="grid grid-cols-3 gap-2">
                            <button data-level="low" class="level-btn selected px-3 py-3 rounded-xl text-sm font-medium border-2 border-gray-200 dark:border-gray-700 text-center">
                                <span class="block text-lg">🎬</span>
                                <span class="block mt-1 font-semibold">Low</span>
                                <span class="block text-xs opacity-70">High Quality</span>
                            </button>
                            <button data-level="medium" class="level-btn px-3 py-3 rounded-xl text-sm font-medium border-2 border-gray-200 dark:border-gray-700 bg-white dark:bg-gray-800 text-gray-600 dark:text-gray-400 text-center">
                                <span class="block text-lg">⚖️</span>
                                <span class="block mt-1 font-semibold">Medium</span>
                                <span class="block text-xs opacity-70">Balanced</span>
                            </button>
                            <button data-level="high" class="level-btn px-3 py-3 rounded-xl text-sm font-medium border-2 border-gray-200 dark:border-gray-700 bg-white dark:bg-gray-800 text-gray-600 dark:text-gray-400 text-center">
                                <span class="block text-lg">📦</span>
                                <span class="block mt-1 font-semibold">High</span>
                                <span class="block text-xs opacity-70">Smallest</span>
                            </button>
                        </div>
                    </div>
                    <div class="p-4 rounded-2xl bg-gray-50 dark:bg-gray-800/50">
                        <p class="font-medium text-gray-900 dark:text-white mb-2">Output Format</p>
                        <select id="outputFormat" class="w-full sm:w-48 px-4 py-2.5 rounded-xl border border-gray-300 dark:border-gray-600 bg-white dark:bg-gray-800 text-gray-900 dark:text-white text-sm focus:ring-2 focus:ring-brand-500 outline-none">
                            <option value="mp4" selected>MP4 (Recommended)</option>
                            <option value="webm">WebM</option>
                        </select>
                    </div>
                </div>

                <!-- Large File Warning -->
                <div id="largeWarn" class="hidden p-4 rounded-2xl bg-amber-50 dark:bg-amber-900/20 border border-amber-200 dark:border-amber-800">
                    <div class="flex items-start space-x-3">
                        <svg class="w-5 h-5 text-amber-600 dark:text-amber-400 mt-0.5 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-2.5L13.732 4c-.77-.833-1.964-.833-2.732 0L3.34 16.5c-.77.833.192 2.5 1.732 2.5z"/></svg>
                        <div>
                            <p class="font-medium text-amber-800 dark:text-amber-300">Large File Detected</p>
                            <p class="text-sm text-amber-700 dark:text-amber-400 mt-1">Processing may take several minutes. Keep this tab open and active.</p>
                        </div>
                    </div>
                </div>

                <!-- Process Button -->
                <button id="processBtn" class="w-full py-4 px-6 rounded-2xl font-semibold text-white bg-gradient-to-r from-brand-600 to-brand-500 hover:from-brand-700 hover:to-brand-600 shadow-lg shadow-brand-500/25 hover:shadow-brand-500/40 transition-all duration-300 transform hover:scale-[1.01] active:scale-[0.99] disabled:opacity-50 disabled:cursor-not-allowed disabled:transform-none disabled:shadow-none flex items-center justify-center space-x-2">
                    <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg>
                    <span>Process Video</span>
                </button>
            </div>
        </div>
    </div>

    <!-- PROCESSING PANEL -->
    <div id="processingPanel" class="hidden mt-6 slide-up">
        <div class="bg-white dark:bg-gray-900 rounded-3xl shadow-xl border border-gray-100 dark:border-gray-800 p-8">
            <div class="text-center space-y-6">
                <div class="relative mx-auto w-20 h-20">
                    <div class="absolute inset-0 rounded-full bg-brand-100 dark:bg-brand-900/30 animate-ping opacity-20"></div>
                    <div class="w-20 h-20 rounded-full bg-brand-100 dark:bg-brand-900/30 flex items-center justify-center">
                        <svg class="w-10 h-10 text-brand-600 dark:text-brand-400 animate-spin" fill="none" viewBox="0 0 24 24"><circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle><path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path></svg>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-gray-900 dark:text-white">Processing Your Video</h3>
                    <p id="procStatus" class="mt-2 text-sm text-gray-500 dark:text-gray-400">Initializing...</p>
                </div>
                <div class="max-w-md mx-auto">
                    <div class="flex justify-between text-sm font-medium text-gray-600 dark:text-gray-400 mb-2">
                        <span>Progress</span>
                        <span id="procPercent">0%</span>
                    </div>
                    <div class="h-3 bg-gray-200 dark:bg-gray-700 rounded-full overflow-hidden">
                        <div id="procBar" class="h-full progress-fill rounded-full" style="width:0%"></div>
                    </div>
                </div>
                <div id="procLog" class="log-container text-xs text-gray-400 dark:text-gray-500 font-mono bg-gray-50 dark:bg-gray-800/50 rounded-xl p-3 max-h-28 overflow-y-auto text-left space-y-0.5">
                    <p>Waiting for engine...</p>
                </div>
            </div>
        </div>
    </div>

    <!-- RESULTS PANEL -->
    <div id="resultsPanel" class="hidden mt-6 slide-up">
        <div class="bg-white dark:bg-gray-900 rounded-3xl shadow-xl border border-gray-100 dark:border-gray-800 overflow-hidden">
            <div class="p-6 bg-gradient-to-r from-green-50 to-emerald-50 dark:from-green-900/20 dark:to-emerald-900/20 border-b border-green-100 dark:border-green-800/30">
                <div class="flex items-center space-x-3">
                    <div class="w-12 h-12 rounded-full bg-green-100 dark:bg-green-900/30 flex items-center justify-center">
                        <svg class="w-6 h-6 text-green-600 dark:text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
                    </div>
                    <div>
                        <h3 class="text-lg font-semibold text-green-900 dark:text-green-300">Processing Complete!</h3>
                        <p class="text-sm text-green-700 dark:text-green-400">Your video has been optimized successfully</p>
                    </div>
                </div>
            </div>
            <div class="p-6 space-y-4">
                <div class="grid grid-cols-3 gap-3">
                    <div class="p-4 rounded-2xl bg-gray-50 dark:bg-gray-800/50 text-center">
                        <p class="text-xs font-medium text-gray-500 dark:text-gray-400 uppercase tracking-wider">Original</p>
                        <p class="text-xl font-bold text-gray-900 dark:text-white mt-1" id="resOriginal">--</p>
                    </div>
                    <div class="p-4 rounded-2xl bg-brand-50 dark:bg-brand-900/20 text-center">
                        <p class="text-xs font-medium text-brand-600 dark:text-brand-400 uppercase tracking-wider">New Size</p>
                        <p class="text-xl font-bold text-brand-700 dark:text-brand-300 mt-1" id="resNew">--</p>
                    </div>
                    <div class="p-4 rounded-2xl bg-green-50 dark:bg-green-900/20 text-center">
                        <p class="text-xs font-medium text-green-600 dark:text-green-400 uppercase tracking-wider">Saved</p>
                        <p class="text-xl font-bold text-green-700 dark:text-green-300 mt-1" id="resSaved">--</p>
                    </div>
                </div>
                <div class="p-4 rounded-2xl bg-gray-50 dark:bg-gray-800/50">
                    <p class="font-medium text-gray-900 dark:text-white mb-2">What was done:</p>
                    <ul id="resList" class="space-y-1 text-sm text-gray-600 dark:text-gray-400"></ul>
                </div>
                <div class="flex flex-col sm:flex-row gap-3">
                    <button id="downloadBtn" class="flex-1 py-4 px-6 rounded-2xl font-semibold text-white bg-gradient-to-r from-green-600 to-emerald-500 hover:from-green-700 hover:to-emerald-600 shadow-lg shadow-green-500/25 transition-all duration-300 transform hover:scale-[1.01] active:scale-[0.99] flex items-center justify-center space-x-2">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg>
                        <span>Download Optimized Video</span>
                    </button>
                    <button id="anotherBtn" class="py-4 px-6 rounded-2xl font-semibold text-gray-700 dark:text-gray-300 bg-gray-100 dark:bg-gray-800 hover:bg-gray-200 dark:hover:bg-gray-700 transition-colors flex items-center justify-center space-x-2">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6"/></svg>
                        <span>Process Another</span>
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- ERROR PANEL -->
    <div id="errorPanel" class="hidden mt-6 slide-up">
        <div class="bg-white dark:bg-gray-900 rounded-3xl shadow-xl border border-red-200 dark:border-red-800/30 p-6">
            <div class="flex items-start space-x-4">
                <div class="w-12 h-12 rounded-full bg-red-100 dark:bg-red-900/30 flex items-center justify-center flex-shrink-0">
                    <svg class="w-6 h-6 text-red-600 dark:text-red-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                </div>
                <div class="flex-1">
                    <h3 class="text-lg font-semibold text-red-900 dark:text-red-300">Processing Error</h3>
                    <p id="errorMsg" class="mt-1 text-sm text-red-700 dark:text-red-400"></p>
                    <button id="retryBtn" class="mt-4 px-6 py-2 rounded-xl font-medium text-red-700 dark:text-red-300 bg-red-50 dark:bg-red-900/20 hover:bg-red-100 dark:hover:bg-red-900/40 transition-colors">Try Again</button>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- FOOTER -->
<footer class="border-t border-gray-200 dark:border-gray-800 bg-white dark:bg-gray-900 transition-colors">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 py-8 text-center">
        <p class="text-sm text-gray-500 dark:text-gray-400">All processing happens in your browser. Your files never leave your device.</p>
        <p class="text-xs text-gray-400 dark:text-gray-500 mt-2">Powered by FFmpeg.wasm • Built for privacy-conscious users</p>
    </div>
</footer>

<!-- ============ JAVASCRIPT ============ -->
<script type="module">

// ==============================================
// UTILITIES
// ==============================================
function formatBytes(bytes, d = 2) {
    if (!bytes || bytes === 0) return '0 Bytes';
    const k = 1024, s = ['Bytes','KB','MB','GB'];
    const i = Math.floor(Math.log(bytes) / Math.log(k));
    return parseFloat((bytes / Math.pow(k, i)).toFixed(d)) + ' ' + s[i];
}

function formatDuration(sec) {
    if (!sec || isNaN(sec)) return '0:00';
    const h = Math.floor(sec / 3600), m = Math.floor((sec % 3600) / 60), s = Math.floor(sec % 60);
    return h > 0 ? `${h}:${String(m).padStart(2,'0')}:${String(s).padStart(2,'0')}` : `${m}:${String(s).padStart(2,'0')}`;
}

function calcReduction(orig, comp) {
    if (!orig || orig === 0) return '0%';
    const r = ((orig - comp) / orig) * 100;
    return (r < 0 ? '+' + Math.abs(r).toFixed(1) : r.toFixed(1)) + '%';
}

function getExt(name) { return name.split('.').pop().toLowerCase(); }
function baseName(name) { return name.substring(0, name.lastIndexOf('.')) || name; }

function validateFile(file) {
    const ok = ['mp4','mov','avi','mkv'];
    const ext = getExt(file.name);
    if (!ok.includes(ext) && !file.type.startsWith('video/')) return { valid: false, error: `Unsupported format "${ext.toUpperCase()}". Use MP4, MOV, AVI, or MKV.` };
    if (file.size > 2 * 1024 * 1024 * 1024) return { valid: false, error: `File too large (${formatBytes(file.size)}). Maximum is 2GB.` };
    if (file.size === 0) return { valid: false, error: 'File appears empty.' };
    return { valid: true };
}

function getVideoDuration(file) {
    return new Promise(resolve => {
        const v = document.createElement('video');
        v.preload = 'metadata';
        v.onloadedmetadata = () => { URL.revokeObjectURL(v.src); resolve(v.duration); };
        v.onerror = () => { URL.revokeObjectURL(v.src); resolve(0); };
        v.src = URL.createObjectURL(file);
    });
}

// ==============================================
// THEME
// ==============================================
const themeKey = 'vo-theme';
function initTheme() {
    const saved = localStorage.getItem(themeKey);
    const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
    if (saved === 'dark' || (!saved && prefersDark)) document.documentElement.classList.add('dark');
    else document.documentElement.classList.remove('dark');
}
initTheme();
document.getElementById('themeBtn').addEventListener('click', () => {
    const isDark = document.documentElement.classList.toggle('dark');
    localStorage.setItem(themeKey, isDark ? 'dark' : 'light');
});

// ==============================================
// DOM REFS
// ==============================================
const $ = id => document.getElementById(id);
const dropZone = $('dropZone');
const fileInput = $('fileInput');
const filePanel = $('filePanel');
const processingPanel = $('processingPanel');
const resultsPanel = $('resultsPanel');
const errorPanel = $('errorPanel');
const processBtn = $('processBtn');
const metadataToggle = $('metadataToggle');
const compressToggle = $('compressToggle');
const compressOptions = $('compressOptions');
const engineBadge = $('engineBadge');

// ==============================================
// STATE
// ==============================================
let currentFile = null;
let currentFileUrl = null;
let outputBlob = null;
let outputUrl = null;
let outputName = '';
let ffmpegInstance = null;
let ffmpegLoaded = false;
let isProcessing = false;
let metadataEnabled = true;
let compressEnabled = false;
let compressionLevel = 'low';

// ==============================================
// TOGGLE LOGIC
// ==============================================
$('metadataToggleRow').addEventListener('click', (e) => {
    if (e.target.closest('#metadataToggle') || e.target.closest('#metadataToggleRow')) {
        metadataEnabled = !metadataEnabled;
        metadataToggle.classList.toggle('active', metadataEnabled);
    }
});

$('compressToggleRow').addEventListener('click', (e) => {
    if (e.target.closest('#compressToggle') || e.target.closest('#compressToggleRow')) {
        compressEnabled = !compressEnabled;
        compressToggle.classList.toggle('active', compressEnabled);
        compressOptions.classList.toggle('hidden', !compressEnabled);
    }
});

// Level buttons
document.querySelectorAll('.level-btn').forEach(btn => {
    btn.addEventListener('click', () => {
        document.querySelectorAll('.level-btn').forEach(b => {
            b.classList.remove('selected');
            b.classList.add('bg-white', 'dark:bg-gray-800', 'text-gray-600', 'dark:text-gray-400');
        });
        btn.classList.add('selected');
        btn.classList.remove('bg-white', 'dark:bg-gray-800', 'text-gray-600', 'dark:text-gray-400');
        compressionLevel = btn.dataset.level;
    });
});

// ==============================================
// FILE HANDLING
// ==============================================
function cleanup() {
    if (currentFileUrl) { URL.revokeObjectURL(currentFileUrl); currentFileUrl = null; }
    if (outputUrl) { URL.revokeObjectURL(outputUrl); outputUrl = null; }
    outputBlob = null; outputName = '';
}

async function handleFile(file) {
    const v = validateFile(file);
    if (!v.valid) { showError(v.error); return; }

    cleanup();
    currentFile = file;
    currentFileUrl = URL.createObjectURL(file);

    const duration = await getVideoDuration(file);

    $('dispFileName').textContent = file.name;
    $('dispFileSize').textContent = formatBytes(file.size);
    $('dispDuration').textContent = formatDuration(duration);
    $('dispFormat').textContent = getExt(file.name).toUpperCase();

    $('videoPreview').src = currentFileUrl;
    $('largeWarn').classList.toggle('hidden', file.size < 100 * 1024 * 1024);

    hideAll();
    filePanel.classList.remove('hidden');
    setTimeout(() => filePanel.scrollIntoView({ behavior: 'smooth', block: 'start' }), 100);
}

// Drop zone events
dropZone.addEventListener('click', () => fileInput.click());
$('heroUploadBtn').addEventListener('click', () => fileInput.click());

fileInput.addEventListener('change', e => {
    if (e.target.files.length) handleFile(e.target.files[0]);
});

['dragenter','dragover'].forEach(ev => {
    dropZone.addEventListener(ev, e => { e.preventDefault(); e.stopPropagation(); dropZone.classList.add('drag-active'); });
});
['dragleave','drop'].forEach(ev => {
    dropZone.addEventListener(ev, e => { e.preventDefault(); e.stopPropagation(); dropZone.classList.remove('drag-active'); });
});
dropZone.addEventListener('drop', e => {
    if (e.dataTransfer.files.length) handleFile(e.dataTransfer.files[0]);
});
document.addEventListener('dragover', e => e.preventDefault());
document.addEventListener('drop', e => e.preventDefault());

$('removeFileBtn').addEventListener('click', e => {
    e.stopPropagation();
    currentFile = null;
    cleanup();
    fileInput.value = '';
    $('videoPreview').src = '';
    filePanel.classList.add('hidden');
    hideAll();
});

// ==============================================
// PANEL HELPERS
// ==============================================
function hideAll() {
    processingPanel.classList.add('hidden');
    resultsPanel.classList.add('hidden');
    errorPanel.classList.add('hidden');
}

function showError(msg) {
    hideAll();
    $('errorMsg').textContent = msg;
    errorPanel.classList.remove('hidden');
    errorPanel.scrollIntoView({ behavior: 'smooth', block: 'center' });
    resetProcessBtn();
}

function resetProcessBtn() {
    processBtn.disabled = false;
    processBtn.innerHTML = '<svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg><span>Process Video</span>';
}

function setProgress(pct, status) {
    $('procBar').style.width = pct + '%';
    $('procPercent').textContent = Math.round(pct) + '%';
    if (status) $('procStatus').textContent = status;
}

function addLog(msg) {
    const el = $('procLog');
    const p = document.createElement('p');
    p.textContent = msg;
    el.appendChild(p);
    el.scrollTop = el.scrollHeight;
    while (el.children.length > 60) el.removeChild(el.firstChild);
}

// ==============================================
// FFMPEG LOADING
// ==============================================
async function loadFFmpeg() {
    engineBadge.classList.remove('hidden');
    $('engineBadgeText').textContent = 'Loading engine...';

    try {
        const { FFmpeg } = await import('https://cdn.jsdelivr.net/npm/@ffmpeg/ffmpeg@0.12.10/+esm');
        const { toBlobURL } = await import('https://cdn.jsdelivr.net/npm/@ffmpeg/util@0.12.1/+esm');

        ffmpegInstance = new FFmpeg();

        ffmpegInstance.on('log', ({ message }) => {
            if (isProcessing) addLog(message);
        });

        ffmpegInstance.on('progress', ({ progress }) => {
            if (isProcessing && progress > 0 && progress <= 1) {
                const pct = Math.min(Math.round(progress * 100), 99);
                setProgress(pct, pct < 30 ? 'Analyzing video...' : pct < 70 ? 'Processing frames...' : 'Finalizing...');
            }
        });

        const coreBase = 'https://cdn.jsdelivr.net/npm/@ffmpeg/core@0.12.6/dist/umd';

        await ffmpegInstance.load({
            coreURL: await toBlobURL(`${coreBase}/ffmpeg-core.js`, 'text/javascript'),
            wasmURL: await toBlobURL(`${coreBase}/ffmpeg-core.wasm`, 'application/wasm'),
        });

        ffmpegLoaded = true;
        engineBadge.className = 'hidden sm:flex items-center px-3 py-1.5 rounded-full text-xs font-medium bg-green-100 dark:bg-green-900/30 text-green-700 dark:text-green-400';
        $('engineBadgeText').textContent = 'Engine ready';
        engineBadge.querySelector('span:first-child').className = 'w-2 h-2 rounded-full bg-green-500 mr-2';

        setTimeout(() => {
            engineBadge.style.transition = 'opacity 0.5s';
            engineBadge.style.opacity = '0';
            setTimeout(() => engineBadge.classList.add('hidden'), 500);
        }, 3000);

    } catch (err) {
        console.error('FFmpeg load error:', err);
        engineBadge.className = 'hidden sm:flex items-center px-3 py-1.5 rounded-full text-xs font-medium bg-red-100 dark:bg-red-900/30 text-red-700 dark:text-red-400';
        $('engineBadgeText').textContent = 'Engine failed';
        engineBadge.querySelector('span:first-child').className = 'w-2 h-2 rounded-full bg-red-500 mr-2';
    }
}

// ==============================================
// PROCESSING
// ==============================================
async function processVideo() {
    if (isProcessing || !currentFile) return;

    if (!metadataEnabled && !compressEnabled) {
        showError('Please enable at least one option: Remove Metadata or Compress Video.');
        return;
    }

    if (!ffmpegLoaded) {
        showError('Processing engine is still loading. Please wait a moment and try again.');
        return;
    }

    isProcessing = true;
    hideAll();

    processBtn.disabled = true;
    processBtn.innerHTML = '<svg class="w-5 h-5 animate-spin" fill="none" viewBox="0 0 24 24"><circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle><path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path></svg><span>Processing...</span>';

    setProgress(0, 'Initializing...');
    $('procLog').innerHTML = '<p>Starting processing...</p>';
    processingPanel.classList.remove('hidden');
    processingPanel.scrollIntoView({ behavior: 'smooth', block: 'center' });

    const fmt = $('outputFormat').value || 'mp4';
    const inExt = getExt(currentFile.name);
    const inName = `input.${inExt}`;
    const outName = `output.${fmt}`;

    try {
        // Write input file
        setProgress(2, 'Loading file into memory...');
        addLog(`Input: ${currentFile.name} (${formatBytes(currentFile.size)})`);

        const { fetchFile } = await import('https://cdn.jsdelivr.net/npm/@ffmpeg/util@0.12.1/+esm');
        const fileData = await fetchFile(currentFile);
        await ffmpegInstance.writeFile(inName, fileData);

        setProgress(5, 'Building processing pipeline...');

        // Build args
        const args = ['-i', inName];

        if (metadataEnabled) {
            args.push('-map_metadata', '-1', '-map_chapters', '-1');
            addLog('Metadata stripping enabled');
        }

        if (compressEnabled) {
            addLog(`Compression: ${compressionLevel} quality`);

            if (fmt === 'webm') {
                const crfMap = { low: '30', medium: '36', high: '42' };
                args.push('-c:v', 'libvpx-vp9', '-crf', crfMap[compressionLevel], '-b:v', '0');
                args.push('-c:a', 'libopus', '-b:a', compressionLevel === 'high' ? '64k' : '128k');
            } else {
                const crfMap = { low: '22', medium: '28', high: '34' };
                const presetMap = { low: 'slow', medium: 'medium', high: 'fast' };
                const abMap = { low: '192k', medium: '128k', high: '96k' };

                args.push('-c:v', 'libx264', '-crf', crfMap[compressionLevel]);
                args.push('-preset', presetMap[compressionLevel]);
                args.push('-pix_fmt', 'yuv420p');
                args.push('-movflags', '+faststart');

                if (compressionLevel === 'high') {
                    args.push('-vf', 'scale=trunc(iw*3/4/2)*2:trunc(ih*3/4/2)*2');
                    addLog('Resolution scaled to 75% for maximum compression');
                }

                args.push('-c:a', 'aac', '-b:a', abMap[compressionLevel], '-ac', '2');
            }
        } else {
            args.push('-c', 'copy');
        }

        args.push('-y', outName);

        addLog(`Command: ffmpeg ${args.join(' ')}`);
        setProgress(8, 'Processing video...');

        // Execute
        await ffmpegInstance.exec(args);

        setProgress(95, 'Reading output...');

        // Read output
        const data = await ffmpegInstance.readFile(outName);
        const mimeMap = { mp4: 'video/mp4', webm: 'video/webm', avi: 'video/x-msvideo' };

        if (outputUrl) URL.revokeObjectURL(outputUrl);
        outputBlob = new Blob([data.buffer], { type: mimeMap[fmt] || 'video/mp4' });
        outputUrl = URL.createObjectURL(outputBlob);

        const metaOnly = metadataEnabled && !compressEnabled;
        outputName = `${baseName(currentFile.name)}${metaOnly ? '_clean' : '_optimized'}.${fmt}`;

        addLog(`Output: ${outputName} (${formatBytes(outputBlob.size)})`);

        // Cleanup ffmpeg fs
        try { await ffmpegInstance.deleteFile(inName); } catch(e) {}
        try { await ffmpegInstance.deleteFile(outName); } catch(e) {}

        setProgress(100, 'Complete!');

        // Show results
        setTimeout(() => {
            showResults(currentFile.size, outputBlob.size);
        }, 500);

    } catch (err) {
        console.error('Processing error:', err);
        try { await ffmpegInstance.deleteFile(inName); } catch(e) {}
        try { await ffmpegInstance.deleteFile(outName); } catch(e) {}
        showError(err.message || 'Processing failed. The file may be corrupted or use an unsupported codec.');
    } finally {
        isProcessing = false;
        resetProcessBtn();
    }
}

function showResults(origSize, newSize) {
    hideAll();
    $('resOriginal').textContent = formatBytes(origSize);
    $('resNew').textContent = formatBytes(newSize);
    $('resSaved').textContent = calcReduction(origSize, newSize);

    const list = $('resList');
    list.innerHTML = '';
    const items = [];
    if (metadataEnabled) items.push('✅ All metadata stripped (GPS, camera info, timestamps)');
    if (compressEnabled) {
        items.push('✅ Re-encoded with H.264 codec');
        const labels = { low: 'Low (High Quality)', medium: 'Medium (Balanced)', high: 'High (Max Compression)' };
        items.push(`✅ Compression: ${labels[compressionLevel]}`);
        items.push('✅ Audio optimized with AAC');
    }
    items.push(`✅ Output: ${($('outputFormat').value || 'mp4').toUpperCase()}`);

    items.forEach(text => {
        const li = document.createElement('li');
        li.textContent = text;
        li.className = 'py-0.5';
        list.appendChild(li);
    });

    resultsPanel.classList.remove('hidden');
    resultsPanel.scrollIntoView({ behavior: 'smooth', block: 'center' });

    // Auto download
    setTimeout(() => triggerDownload(), 800);
}

function triggerDownload() {
    if (!outputBlob || !outputUrl) return;
    const a = document.createElement('a');
    a.href = outputUrl;
    a.download = outputName;
    document.body.appendChild(a);
    a.click();
    document.body.removeChild(a);
}

// ==============================================
// BUTTON EVENTS
// ==============================================
processBtn.addEventListener('click', processVideo);

$('downloadBtn').addEventListener('click', triggerDownload);

$('anotherBtn').addEventListener('click', () => {
    currentFile = null;
    cleanup();
    fileInput.value = '';
    $('videoPreview').src = '';
    filePanel.classList.add('hidden');
    hideAll();
    metadataEnabled = true; compressEnabled = false; compressionLevel = 'low';
    metadataToggle.classList.add('active');
    compressToggle.classList.remove('active');
    compressOptions.classList.add('hidden');
    document.querySelectorAll('.level-btn').forEach((b, i) => {
        if (i === 0) { b.classList.add('selected'); b.classList.remove('bg-white','dark:bg-gray-800','text-gray-600','dark:text-gray-400'); }
        else { b.classList.remove('selected'); b.classList.add('bg-white','dark:bg-gray-800','text-gray-600','dark:text-gray-400'); }
    });
    $('outputFormat').value = 'mp4';
    window.scrollTo({ top: 0, behavior: 'smooth' });
});

$('retryBtn').addEventListener('click', () => {
    hideAll();
    if (currentFile) processVideo();
});

// ==============================================
// INIT
// ==============================================
loadFFmpeg();

</script>
</body>
</html>