<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100">
    <div class="flex h-screen">
        <!-- Sidebar -->
        <div class="w-64 bg-blue-900 text-white p-5">
            <h1 class="text-xl font-bold mb-5">Dashboard</h1>
            <ul>
                <li class="mb-3"><a href="#" class="hover:text-gray-300">Home</a></li>
                <li class="mb-3"><a href="#" class="hover:text-gray-300">Analytics</a></li>
                <li class="mb-3"><a href="#" class="hover:text-gray-300">Settings</a></li>
            </ul>
        </div>
        
        <!-- Main Content -->
        <div class="flex-1 p-6">
            <h2 class="text-2xl font-semibold mb-4">Selamat Datang!</h2>
            <div class="grid grid-cols-3 gap-4">
                <div class="bg-white p-4 rounded-lg shadow-md">
                    <h3 class="text-lg font-bold">Statistik 1</h3>
                    <p class="text-gray-600">Data 1</p>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md">
                    <h3 class="text-lg font-bold">Statistik 2</h3>
                    <p class="text-gray-600">Data 2</p>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md">
                    <h3 class="text-lg font-bold">Statistik 3</h3>
                    <p class="text-gray-600">Data 3</p>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
