[Uploading index.html.txt…]()
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>戴嘉樟 | 屏東科技大學工業管理</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 引入 Lucide 圖標庫 -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/lucide/0.263.0/lucide.min.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;500;700&display=swap');
        body {
            font-family: 'Noto Sans TC', sans-serif;
            scroll-behavior: smooth;
        }
        .hero-gradient {
            background: linear-gradient(135deg, #1e293b 0%, #334155 100%);
        }
        .card-hover:hover {
            transform: translateY(-5px);
            transition: all 0.3s ease;
        }
        .file-upload-dash {
            border: 2px dashed #cbd5e1;
            transition: all 0.3s ease;
        }
        .file-upload-dash:hover {
            border-color: #3b82f6;
            background-color: #f8fafc;
        }
        /* 照片顯示優化 */
        .profile-container {
            position: relative;
            width: 100%;
            max-width: 380px;
        }
        .profile-img {
            width: 100%;
            height: auto;
            border-radius: 2rem;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.4);
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            object-fit: cover;
            border: 4px solid white;
        }
        .profile-img:hover {
            transform: scale(1.03) rotate(1deg);
        }
        .profile-fallback {
            background: linear-gradient(135deg, #e2e8f0 0%, #cbd5e1 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            color: #64748b;
            min-height: 500px;
            border-radius: 2rem;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-900">

    <!-- 導航列 -->
    <nav class="fixed w-full z-50 bg-white/80 backdrop-blur-md border-b border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <div class="flex-shrink-0 font-bold text-2xl text-blue-900 tracking-tighter">
                    戴嘉樟
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#home" class="text-slate-600 hover:text-blue-600 font-medium transition">首頁</a>
                        <a href="#about" class="text-slate-600 hover:text-blue-600 font-medium transition">關於我</a>
                        <a href="#knowledge" class="text-slate-600 hover:text-blue-600 font-medium transition">工作研究</a>
                        <a href="#assignment" class="text-slate-600 hover:text-blue-600 font-medium transition">作業繳交</a>
                        <a href="#skills" class="text-slate-600 hover:text-blue-600 font-medium transition">專業技能</a>
                        <a href="#contact" class="bg-blue-900 text-white px-5 py-2 rounded-xl hover:bg-blue-800 transition shadow-md shadow-blue-900/20">聯絡我</a>
                    </div>
                </div>
            </div>
        </div>
    </nav>

    <!-- 英雄區 -->
    <section id="home" class="hero-gradient min-h-screen flex items-center pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24 text-center">
            <div class="inline-block px-4 py-1.5 mb-6 text-sm font-bold tracking-widest text-blue-400 uppercase bg-blue-400/10 rounded-full">
                Industrial Engineering & Management
            </div>
            <h1 class="text-4xl md:text-7xl font-extrabold text-white mb-8 leading-tight">
                追求卓越效率<br><span class="text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-emerald-400">優化產業系統</span>
            </h1>
            <p class="text-xl text-slate-300 mb-10 max-w-2xl mx-auto leading-relaxed">
                我是 戴嘉樟，目前就讀於國立屏東科技大學工業管理系。致力於運用工業工程技術提昇生產力與品質管理，創造更高效的運作模式。
            </p>
            <div class="flex flex-col sm:flex-row justify-center items-center gap-4">
                <a href="#knowledge" class="w-full sm:w-auto bg-blue-600 text-white px-10 py-4 rounded-full font-bold hover:bg-blue-500 transition-all transform hover:scale-105 shadow-lg shadow-blue-600/30">
                    查看專業知識庫
                </a>
                <a href="#assignment" class="w-full sm:w-auto bg-white/10 text-white border border-white/20 px-10 py-4 rounded-full font-bold hover:bg-white/20 transition-all backdrop-blur-sm">
                    進入繳交區
                </a>
            </div>
        </div>
    </section>

    <!-- 關於我 -->
    <section id="about" class="py-32 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <!-- 個人照片展示 -->
                <div class="flex justify-center order-2 md:order-1">
                    <div class="profile-container group">
                        <!-- 背景裝飾光環 -->
                        <div class="absolute -inset-4 bg-gradient-to-tr from-blue-600 to-emerald-400 rounded-[2.5rem] blur opacity-20 group-hover:opacity-30 transition duration-1000"></div>
                        
                        <!-- 實體照片區塊 -->
                        <div class="relative">
                            <!-- 使用上傳的照片檔名 -->
                            <img src="大頭照.jpg" alt="戴嘉樟 個人照片" 
                                 onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
                                 class="profile-img">
                            
                            <!-- 載入失敗時的備用顯示 -->
                            <div class="profile-fallback hidden">
                                <i data-lucide="user-circle" class="w-24 h-24 mb-4 opacity-30"></i>
                                <p class="font-bold text-slate-500 text-lg">戴嘉樟</p>
                                <p class="text-sm text-slate-400">國立屏東科技大學</p>
                            </div>

                            <!-- 裝飾標籤 -->
                            <div class="absolute -bottom-8 -left-8 bg-white p-5 rounded-2xl shadow-2xl border border-slate-100 hidden lg:block">
                                <div class="flex items-center space-x-3">
                                    <div class="w-10 h-10 bg-blue-50 rounded-lg flex items-center justify-center">
                                        <i data-lucide="award" class="w-6 h-6 text-blue-600"></i>
                                    </div>
                                    <div>
                                        <p class="text-xs text-slate-400 font-bold uppercase tracking-wider">Education</p>
                                        <p class="text-sm font-black text-slate-800">NPUST IEM</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="space-y-10 order-1 md:order-2">
                    <div class="space-y-4">
                        <h2 class="text-5xl font-black text-slate-900 tracking-tighter">關於我</h2>
                        <div class="w-20 h-2 bg-blue-600 rounded-full"></div>
                    </div>
                    
                    <p class="text-xl text-slate-600 leading-relaxed italic border-l-4 border-blue-600 pl-8 py-2">
                        「工業工程師是產業的醫師」，我深信透過科學化的數據分析與流程改善，能夠為任何複雜的系統找出最佳化解決方案。
                    </p>

                    <p class="text-lg text-slate-600 leading-relaxed">
                        我是 <span class="font-bold text-slate-900 text-xl">戴嘉樟</span>，目前於國立屏東科技大學工業管理系深造。在學習過程中，我對工作研究、生產計劃及品質管制展現了深厚興趣，並致力於實務應用。
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div class="flex items-center p-4 bg-slate-50 rounded-2xl border border-slate-100 card-hover">
                            <i data-lucide="check-circle" class="text-blue-600 w-6 h-6 mr-3"></i>
                            <span class="font-bold text-slate-700">生產管理與管制</span>
                        </div>
                        <div class="flex items-center p-4 bg-slate-50 rounded-2xl border border-slate-100 card-hover">
                            <i data-lucide="check-circle" class="text-blue-600 w-6 h-6 mr-3"></i>
                            <span class="font-bold text-slate-700">Six Sigma 品質管理</span>
                        </div>
                        <div class="flex items-center p-4 bg-slate-50 rounded-2xl border border-slate-100 card-hover">
                            <i data-lucide="check-circle" class="text-blue-600 w-6 h-6 mr-3"></i>
                            <span class="font-bold text-slate-700">作業研究 (OR)</span>
                        </div>
                        <div class="flex items-center p-4 bg-slate-50 rounded-2xl border border-slate-100 card-hover">
                            <i data-lucide="check-circle" class="text-blue-600 w-6 h-6 mr-3"></i>
                            <span class="font-bold text-slate-700">工作研究 (Work Study)</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 知識庫與繳交區 -->
    <section id="knowledge" class="py-24 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-black text-slate-900">工作研究核心領域</h2>
                <p class="mt-4 text-slate-600 text-lg">透過「方法研究」與「工作衡量」達到生產效率極大化</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 card-hover">
                    <div class="w-16 h-16 bg-blue-100 rounded-2xl flex items-center justify-center mb-6 text-blue-600">
                        <i data-lucide="settings-2" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-2xl font-bold mb-4">方法研究</h3>
                    <ul class="text-slate-600 space-y-4">
                        <li class="flex items-start"><span class="text-blue-500 mr-3">•</span> 流程圖與程序圖深度分析</li>
                        <li class="flex items-start"><span class="text-blue-500 mr-3">•</span> 動作經濟原則實務應用</li>
                        <li class="flex items-start"><span class="text-blue-500 mr-3">•</span> ECRS 改善手法實踐</li>
                    </ul>
                </div>

                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 card-hover">
                    <div class="w-16 h-16 bg-emerald-100 rounded-2xl flex items-center justify-center mb-6 text-emerald-600">
                        <i data-lucide="clock" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-2xl font-bold mb-4">工作衡量</h3>
                    <ul class="text-slate-600 space-y-4">
                        <li class="flex items-start"><span class="text-emerald-500 mr-3">•</span> 標準工時制定與維護</li>
                        <li class="flex items-start"><span class="text-emerald-500 mr-3">•</span> 寬放時間係數評估</li>
                        <li class="flex items-start"><span class="text-emerald-500 mr-3">•</span> 工作抽查效率分析</li>
                    </ul>
                </div>

                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-100 card-hover">
                    <div class="w-16 h-16 bg-purple-100 rounded-2xl flex items-center justify-center mb-6 text-purple-600">
                        <i data-lucide="activity" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-2xl font-bold mb-4">生產線平衡</h3>
                    <ul class="text-slate-600 space-y-4">
                        <li class="flex items-start"><span class="text-purple-500 mr-3">•</span> 平衡率與損失率計算</li>
                        <li class="flex items-start"><span class="text-purple-500 mr-3">•</span> 瓶頸站點識別與優化</li>
                        <li class="flex items-start"><span class="text-purple-500 mr-3">•</span> 精實看板系統導入</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- 作業繳交區 -->
    <section id="assignment" class="py-32 bg-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-4xl mx-auto">
                <div class="text-center mb-16">
                    <h2 class="text-4xl font-black text-slate-900">作業與專案繳交區</h2>
                    <p class="mt-4 text-slate-600 text-lg">請選擇您的課程並上傳完整報告檔案</p>
                </div>

                <div class="bg-white rounded-[2.5rem] shadow-2xl overflow-hidden border border-white">
                    <div class="p-8 md:p-16">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-10 mb-12">
                            <div class="space-y-4">
                                <label class="block text-sm font-black text-slate-500 uppercase tracking-widest">目標課程名稱</label>
                                <select class="w-full bg-slate-50 border border-slate-200 rounded-2xl px-6 py-4 focus:ring-4 focus:ring-blue-500/10 outline-none transition appearance-none cursor-pointer">
                                    <option>工作研究：組裝作業改善報告</option>
                                    <option>生產計畫：物料需求規劃專案</option>
                                    <option>品質管理：控制圖分析作業</option>
                                    <option>自動化系統：PLC 模擬實作</option>
                                </select>
                            </div>
                            <div class="space-y-4">
                                <label class="block text-sm font-black text-slate-500 uppercase tracking-widest">目前登入學員</label>
                                <div class="flex items-center bg-blue-50/50 border border-blue-100 rounded-2xl px-6 py-4 text-blue-900 font-bold">
                                    <i data-lucide="user" class="w-5 h-5 mr-4 text-blue-400"></i>
                                    <span>戴嘉樟 (gino171709)</span>
                                </div>
                            </div>
                        </div>

                        <!-- 檔案上傳框 -->
                        <div class="file-upload-dash rounded-3xl p-16 text-center cursor-pointer mb-10 group bg-slate-50/50" onclick="document.getElementById('fileInput').click()">
                            <input type="file" id="fileInput" class="hidden" onchange="handleFileSelect(this)">
                            
                            <div id="uploadContent" class="space-y-6">
                                <div class="w-24 h-24 bg-white shadow-lg rounded-full flex items-center justify-center mx-auto group-hover:scale-110 transition duration-500">
                                    <i data-lucide="upload-cloud" class="w-12 h-12 text-blue-600"></i>
                                </div>
                                <div>
                                    <p class="text-slate-900 font-black text-2xl">選擇作業檔案</p>
                                    <p class="text-slate-500 mt-2 font-medium">支援 PDF, Excel, PowerPoint 或 Word 格式</p>
                                </div>
                            </div>

                            <div id="fileSelected" class="hidden">
                                <div class="w-24 h-24 bg-emerald-50 rounded-full flex items-center justify-center mx-auto mb-6">
                                    <i data-lucide="file-check" class="w-12 h-12 text-emerald-500"></i>
                                </div>
                                <p id="fileNameText" class="text-slate-900 font-black text-xl mb-4"></p>
                                <button class="px-6 py-2 bg-slate-200 text-slate-700 rounded-full text-sm font-bold hover:bg-slate-300 transition" onclick="resetFile(event)">更換檔案</button>
                            </div>
                        </div>

                        <button onclick="submitAssignment()" class="w-full bg-blue-900 text-white font-black text-xl py-6 rounded-2xl hover:bg-blue-800 transition-all shadow-xl hover:shadow-blue-900/30 flex items-center justify-center space-x-4">
                            <i data-lucide="check-circle" class="w-6 h-6"></i>
                            <span>確認並送出作業</span>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 聯絡區 -->
    <footer id="contact" class="py-32 bg-slate-900 text-white overflow-hidden relative">
        <!-- 裝飾元素 -->
        <div class="absolute top-0 right-0 -translate-y-1/2 translate-x-1/2 w-96 h-96 bg-blue-600/10 rounded-full blur-3xl"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center relative z-10">
            <h2 class="text-5xl font-black mb-10 tracking-tighter">與我聯繫</h2>
            <p class="text-slate-400 mb-16 text-xl max-w-2xl mx-auto leading-relaxed">
                正在尋找具備工管專業的實習生或合作夥伴嗎？<br>歡迎直接透過以下方式與我交流。
            </p>
            
            <div class="flex flex-col md:flex-row justify-center items-center gap-8 md:gap-16">
                <a href="mailto:gino171709@gmail.com" class="flex items-center space-x-5 hover:text-blue-400 transition group p-6 bg-white/5 rounded-3xl border border-white/10 w-full md:w-auto">
                    <div class="w-16 h-16 bg-blue-600 rounded-2xl flex items-center justify-center shadow-lg shadow-blue-600/40 group-hover:scale-110 transition">
                        <i data-lucide="mail" class="w-8 h-8"></i>
                    </div>
                    <div class="text-left">
                        <p class="text-xs font-black uppercase tracking-widest text-slate-500">Email Address</p>
                        <p class="text-xl font-bold">gino171709@gmail.com</p>
                    </div>
                </a>
                
                <div class="flex items-center space-x-5 p-6 bg-white/5 rounded-3xl border border-white/10 w-full md:w-auto">
                    <div class="w-16 h-16 bg-emerald-600 rounded-2xl flex items-center justify-center shadow-lg shadow-emerald-600/40">
                        <i data-lucide="map-pin" class="w-8 h-8"></i>
                    </div>
                    <div class="text-left">
                        <p class="text-xs font-black uppercase tracking-widest text-slate-500">Location</p>
                        <p class="text-xl font-bold">屏東縣內埔鄉</p>
                    </div>
                </div>
            </div>
            
            <div class="mt-32 pt-10 border-t border-white/10 text-slate-500 text-sm font-medium">
                <p>© 2024 戴嘉樟 | 國立屏東科技大學 工業管理系</p>
                <p class="mt-2 opacity-50 uppercase tracking-[0.2em] text-[10px]">Optimized for Industrial Efficiency</p>
            </div>
        </div>
    </footer>

    <!-- 彈窗組件 -->
    <div id="customAlert" class="fixed inset-0 bg-slate-900/80 hidden z-[100] flex items-center justify-center px-4 backdrop-blur-md">
        <div class="bg-white rounded-[2.5rem] p-12 max-w-md w-full text-center shadow-2xl scale-90 transition-transform duration-300">
            <div id="alertIcon" class="mb-8"></div>
            <h3 id="alertTitle" class="text-3xl font-black mb-4 text-slate-900"></h3>
            <p id="alertMsg" class="text-slate-600 mb-10 text-lg leading-relaxed font-medium"></p>
            <button onclick="closeAlert()" class="w-full bg-blue-600 text-white font-black py-5 rounded-2xl hover:bg-blue-700 transition shadow-lg shadow-blue-600/20 text-lg">好的，我知道了</button>
        </div>
    </div>

    <script>
        window.onload = function() {
            if (typeof lucide !== 'undefined') {
                lucide.createIcons();
            }
        };

        function handleFileSelect(input) {
            if (input.files && input.files[0]) {
                document.getElementById('uploadContent').classList.add('hidden');
                document.getElementById('fileSelected').classList.remove('hidden');
                document.getElementById('fileNameText').innerText = input.files[0].name;
                lucide.createIcons();
            }
        }

        function resetFile(e) {
            e.stopPropagation();
            const input = document.getElementById('fileInput');
            input.value = '';
            document.getElementById('uploadContent').classList.remove('hidden');
            document.getElementById('fileSelected').classList.add('hidden');
        }

        function submitAssignment() {
            const file = document.getElementById('fileInput').files[0];
            if (!file) {
                showCustomAlert('尚未選擇檔案', '請先點擊上傳區塊選擇您的報告檔案。', 'alert-circle', 'text-amber-500');
                return;
            }
            showCustomAlert('繳交成功！', '您的作業檔案「' + file.name + '」已成功傳送到繳交系統。', 'check-circle-2', 'text-emerald-500');
            resetFile({ stopPropagation: () => {} });
        }

        function showCustomAlert(title, msg, icon = 'check-circle-2', iconColor = 'text-emerald-500') {
            const alert = document.getElementById('customAlert');
            document.getElementById('alertTitle').innerText = title;
            document.getElementById('alertMsg').innerText = msg;
            const iconContainer = document.getElementById('alertIcon');
            iconContainer.innerHTML = `<i data-lucide="${icon}" class="w-24 h-24 ${iconColor} mx-auto"></i>`;
            lucide.createIcons();
            alert.classList.remove('hidden');
            setTimeout(() => {
                alert.firstElementChild.classList.remove('scale-90');
                alert.firstElementChild.classList.add('scale-100');
            }, 10);
        }

        function closeAlert() {
            const alert = document.getElementById('customAlert');
            alert.firstElementChild.classList.add('scale-90');
            alert.firstElementChild.classList.remove('scale-100');
            setTimeout(() => {
                alert.classList.add('hidden');
            }, 200);
        }
    </script>
</body>
</html>
