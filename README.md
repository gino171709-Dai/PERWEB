[index.html.txt](https://github.com/user-attachments/files/26236493/index.html.txt)
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dai Jiazhang | 屏東科技大學工業管理</title>
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
            max-width: 350px;
        }
        .profile-img {
            width: 100%;
            border-radius: 1.5rem;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5);
            transition: transform 0.5s ease;
        }
        .profile-img:hover {
            transform: scale(1.02);
        }
        .profile-fallback {
            background: linear-gradient(135deg, #e2e8f0 0%, #cbd5e1 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            color: #64748b;
            height: 450px;
            border-radius: 1.5rem;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-900">

    <!-- 導航列 -->
    <nav class="fixed w-full z-50 bg-white/80 backdrop-blur-md border-b border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <div class="flex-shrink-0 font-bold text-2xl text-blue-900">
                    Dai Jiazhang
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#home" class="hover:text-blue-600 transition">首頁</a>
                        <a href="#about" class="hover:text-blue-600 transition">關於我</a>
                        <a href="#knowledge" class="hover:text-blue-600 transition">工作研究</a>
                        <a href="#assignment" class="hover:text-blue-600 transition">作業繳交</a>
                        <a href="#skills" class="hover:text-blue-600 transition">專業技能</a>
                        <a href="#contact" class="bg-blue-900 text-white px-4 py-2 rounded-lg hover:bg-blue-800 transition">聯絡我</a>
                    </div>
                </div>
            </div>
        </div>
    </nav>

    <!-- 英雄區 -->
    <section id="home" class="hero-gradient min-h-screen flex items-center pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24 text-center">
            <h1 class="text-4xl md:text-6xl font-extrabold text-white mb-6 leading-tight">
                追求卓越效率<br><span class="text-blue-400">優化產業系統</span>
            </h1>
            <p class="text-xl text-slate-300 mb-8 max-w-2xl mx-auto">
                我是 Dai Jiazhang，目前就讀於國立屏東科技大學工業管理系。致力於運用工業工程技術提昇生產力與品質管理。
            </p>
            <div class="flex justify-center space-x-4">
                <a href="#knowledge" class="bg-blue-600 text-white px-8 py-3 rounded-full font-semibold hover:bg-blue-500 transition">專業知識庫</a>
                <a href="#assignment" class="bg-white/10 text-white border border-white/20 px-8 py-3 rounded-full font-semibold hover:bg-white/20 transition">進入繳交區</a>
            </div>
        </div>
    </section>

    <!-- 關於我 -->
    <section id="about" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <!-- 個人照片展示 -->
                <div class="flex justify-center order-2 md:order-1">
                    <div class="profile-container group">
                        <!-- 背景裝飾 -->
                        <div class="absolute -inset-2 bg-gradient-to-tr from-blue-600 to-indigo-400 rounded-[2rem] blur opacity-20 group-hover:opacity-40 transition duration-1000"></div>
                        
                        <!-- 實體照片區塊 -->
                        <div class="relative">
                            <img src="大頭照.jpg" alt="Dai Jiazhang 個人大頭照" 
                                 onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
                                 class="profile-img object-cover aspect-[9/16]">
                            
                            <!-- 載入失敗時的備用顯示 -->
                            <div class="profile-fallback hidden">
                                <i data-lucide="user-circle" class="w-24 h-24 mb-4 opacity-30"></i>
                                <p class="font-bold text-slate-500 text-lg">Dai Jiazhang</p>
                                <p class="text-sm text-slate-400">工業管理系</p>
                            </div>

                            <!-- 裝飾標籤 -->
                            <div class="absolute -bottom-6 -right-6 bg-white p-4 rounded-2xl shadow-xl border border-slate-100 hidden md:block animate-bounce">
                                <div class="flex items-center space-x-2">
                                    <div class="w-3 h-3 bg-green-500 rounded-full"></div>
                                    <span class="text-sm font-bold text-slate-800">屏科大工管系</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="space-y-8 order-1 md:order-2">
                    <div class="space-y-4">
                        <h2 class="text-4xl font-bold text-slate-900 tracking-tight">關於我</h2>
                        <div class="w-16 h-1.5 bg-blue-600 rounded-full"></div>
                    </div>
                    
                    <p class="text-lg text-slate-600 leading-relaxed italic border-l-4 border-blue-100 pl-6">
                        「工業工程師是產業的醫師」，我深信透過科學化的數據分析與流程改善，能夠為任何系統找出最佳解決方案。
                    </p>

                    <p class="text-lg text-slate-600 leading-relaxed">
                        我是 <b>Dai Jiazhang</b>，目前在屏東科技大學工業管理系鑽研，對於工作研究、生產計畫及品質管制有深厚興趣。我善於利用 AutoCAD 進行空間佈置優化，並能運用統計軟體進行生產數據回歸分析。
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div class="flex items-center p-3 bg-slate-50 rounded-xl border border-slate-100">
                            <i data-lucide="check-circle-2" class="text-blue-600 w-5 h-5 mr-3"></i>
                            <span class="font-medium text-slate-700">生產管理與管制</span>
                        </div>
                        <div class="flex items-center p-3 bg-slate-50 rounded-xl border border-slate-100">
                            <i data-lucide="check-circle-2" class="text-blue-600 w-5 h-5 mr-3"></i>
                            <span class="font-medium text-slate-700">Six Sigma 品質管理</span>
                        </div>
                        <div class="flex items-center p-3 bg-slate-50 rounded-xl border border-slate-100">
                            <i data-lucide="check-circle-2" class="text-blue-600 w-5 h-5 mr-3"></i>
                            <span class="font-medium text-slate-700">作業研究 (OR)</span>
                        </div>
                        <div class="flex items-center p-3 bg-slate-50 rounded-xl border border-slate-100">
                            <i data-lucide="check-circle-2" class="text-blue-600 w-5 h-5 mr-3"></i>
                            <span class="font-medium text-slate-700">工作研究 (Work Study)</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 工作研究知識庫 -->
    <section id="knowledge" class="py-24 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-slate-900">工作研究核心領域</h2>
                <p class="mt-4 text-slate-600">透過「方法研究」與「工作衡量」達到生產效率極大化</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- 方法研究 -->
                <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-100 card-hover">
                    <div class="w-14 h-14 bg-blue-100 rounded-xl flex items-center justify-center mb-6 text-blue-600">
                        <i data-lucide="settings-2" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">方法研究</h3>
                    <ul class="text-slate-600 space-y-3">
                        <li class="flex items-start"><span class="text-blue-500 mr-2">•</span> 流程圖與程序圖深度分析</li>
                        <li class="flex items-start"><span class="text-blue-500 mr-2">•</span> 動作經濟原則實務應用</li>
                        <li class="flex items-start"><span class="text-blue-500 mr-2">•</span> ECRS 改善手法實踐</li>
                    </ul>
                </div>

                <!-- 工作衡量 -->
                <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-100 card-hover">
                    <div class="w-14 h-14 bg-emerald-100 rounded-xl flex items-center justify-center mb-6 text-emerald-600">
                        <i data-lucide="clock" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">工作衡量</h3>
                    <ul class="text-slate-600 space-y-3">
                        <li class="flex items-start"><span class="text-emerald-500 mr-2">•</span> 標準工時制定與維護</li>
                        <li class="flex items-start"><span class="text-emerald-500 mr-2">•</span> 寬放時間係數評估</li>
                        <li class="flex items-start"><span class="text-emerald-500 mr-2">•</span> 工作抽查效率分析</li>
                    </ul>
                </div>

                <!-- 生產優化 -->
                <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-100 card-hover">
                    <div class="w-14 h-14 bg-purple-100 rounded-xl flex items-center justify-center mb-6 text-purple-600">
                        <i data-lucide="activity" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">生產線平衡</h3>
                    <ul class="text-slate-600 space-y-3">
                        <li class="flex items-start"><span class="text-purple-500 mr-2">•</span> 平衡率與損失率計算</li>
                        <li class="flex items-start"><span class="text-purple-500 mr-2">•</span> 瓶頸站點識別與優化</li>
                        <li class="flex items-start"><span class="text-purple-500 mr-2">•</span> 精實看板系統導入</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- 作業繳交區 -->
    <section id="assignment" class="py-24 bg-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-4xl mx-auto">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold text-slate-900">作業與專案繳交區</h2>
                    <p class="mt-4 text-slate-600">請確認您的課程名稱並上傳完整報告檔案</p>
                </div>

                <div class="bg-white rounded-3xl shadow-xl overflow-hidden">
                    <div class="p-8 md:p-12">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-10">
                            <div class="space-y-3">
                                <label class="block text-sm font-bold text-slate-700">目標課程</label>
                                <select class="w-full bg-slate-50 border border-slate-200 rounded-xl px-5 py-3 focus:ring-2 focus:ring-blue-500 outline-none transition">
                                    <option>工作研究：組裝作業改善報告</option>
                                    <option>生產計畫：物料需求規劃專案</option>
                                    <option>品質管理：控制圖分析作業</option>
                                    <option>自動化系統：PLC 模擬實作</option>
                                </select>
                            </div>
                            <div class="space-y-3">
                                <label class="block text-sm font-bold text-slate-700">學員資訊</label>
                                <div class="flex items-center bg-slate-50 border border-slate-200 rounded-xl px-5 py-3 text-slate-600">
                                    <i data-lucide="user" class="w-4 h-4 mr-3 text-slate-400"></i>
                                    <span>Dai Jiazhang (屏科大工管)</span>
                                </div>
                            </div>
                        </div>

                        <!-- 檔案上傳框 -->
                        <div class="file-upload-dash rounded-2xl p-16 text-center cursor-pointer mb-8 group" onclick="document.getElementById('fileInput').click()">
                            <input type="file" id="fileInput" class="hidden" onchange="handleFileSelect(this)">
                            
                            <div id="uploadContent" class="space-y-4">
                                <div class="w-20 h-20 bg-blue-50 rounded-full flex items-center justify-center mx-auto group-hover:bg-blue-100 transition">
                                    <i data-lucide="upload-cloud" class="w-10 h-10 text-blue-600"></i>
                                </div>
                                <div>
                                    <p class="text-slate-800 font-bold text-xl">點擊此處選擇檔案</p>
                                    <p class="text-slate-500 mt-2">支援 PDF, Excel, PowerPoint 或 Word 格式</p>
                                </div>
                            </div>

                            <div id="fileSelected" class="hidden animate-pulse">
                                <i data-lucide="file-check" class="w-16 h-16 text-emerald-500 mx-auto mb-4"></i>
                                <p id="fileNameText" class="text-slate-900 font-extrabold text-lg"></p>
                                <button class="mt-4 px-4 py-2 bg-slate-100 text-slate-600 rounded-lg text-sm font-bold hover:bg-slate-200" onclick="resetFile(event)">更改檔案</button>
                            </div>
                        </div>

                        <button onclick="submitAssignment()" class="w-full bg-blue-900 text-white font-black text-lg py-5 rounded-2xl hover:bg-black transition-all shadow-xl hover:shadow-2xl flex items-center justify-center space-x-3">
                            <i data-lucide="send" class="w-6 h-6"></i>
                            <span>正式繳交作業</span>
                        </button>
                    </div>
                    
                    <div class="bg-blue-50 px-8 py-4 text-center">
                        <p class="text-blue-700 text-sm font-medium flex items-center justify-center">
                            <i data-lucide="shield-check" class="w-4 h-4 mr-2"></i>
                            系統已通過屏科大內部網路安全檢核
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 技能區 -->
    <section id="skills" class="py-24 bg-white border-t border-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-16">專業技能掌握</h2>
            <div class="grid md:grid-cols-2 gap-10">
                <div class="space-y-6">
                    <div>
                        <div class="flex justify-between mb-2 font-medium text-slate-700">
                            <span>AutoCAD / 工程製圖</span>
                            <span>85%</span>
                        </div>
                        <div class="w-full bg-slate-100 rounded-full h-2.5">
                            <div class="bg-blue-600 h-2.5 rounded-full" style="width: 85%"></div>
                        </div>
                    </div>
                    <div>
                        <div class="flex justify-between mb-2 font-medium text-slate-700">
                            <span>數據分析 (Excel/SPSS)</span>
                            <span>90%</span>
                        </div>
                        <div class="w-full bg-slate-100 rounded-full h-2.5">
                            <div class="bg-blue-600 h-2.5 rounded-full" style="width: 90%"></div>
                        </div>
                    </div>
                </div>
                <div class="space-y-6">
                    <div>
                        <div class="flex justify-between mb-2 font-medium text-slate-700">
                            <span>ERP 系統操作</span>
                            <span>80%</span>
                        </div>
                        <div class="w-full bg-slate-100 rounded-full h-2.5">
                            <div class="bg-blue-600 h-2.5 rounded-full" style="width: 80%"></div>
                        </div>
                    </div>
                    <div>
                        <div class="flex justify-between mb-2 font-medium text-slate-700">
                            <span>精實生產 (Lean Production)</span>
                            <span>85%</span>
                        </div>
                        <div class="w-full bg-slate-100 rounded-full h-2.5">
                            <div class="bg-blue-600 h-2.5 rounded-full" style="width: 85%"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 聯絡區 -->
    <section id="contact" class="py-24 bg-slate-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-4xl font-bold mb-8">與我聯繫</h2>
            <p class="text-slate-400 mb-12 text-lg max-w-xl mx-auto">
                如果您對工業工程改進專案感興趣，或有實習機會，歡迎隨時透過電子郵件與我聯繫。
            </p>
            <div class="flex flex-col md:flex-row justify-center items-center space-y-6 md:space-y-0 md:space-x-12">
                <a href="mailto:gino171709@gmail.com" class="flex items-center space-x-3 hover:text-blue-400 transition group">
                    <div class="w-12 h-12 bg-blue-600/20 rounded-xl flex items-center justify-center group-hover:bg-blue-600 transition">
                        <i data-lucide="mail" class="w-6 h-6"></i>
                    </div>
                    <span class="text-xl">gino171709@gmail.com</span>
                </a>
                <div class="flex items-center space-x-3">
                    <div class="w-12 h-12 bg-red-600/20 rounded-xl flex items-center justify-center">
                        <i data-lucide="map-pin" class="w-6 h-6 text-red-500"></i>
                    </div>
                    <span class="text-xl">屏東縣內埔鄉</span>
                </div>
            </div>
            <p class="mt-20 text-slate-600">© 2024 Dai Jiazhang - 國立屏東科技大學 工業管理系</p>
        </div>
    </section>

    <!-- 彈窗組件 -->
    <div id="customAlert" class="fixed inset-0 bg-black/60 hidden z-[100] flex items-center justify-center px-4 backdrop-blur-sm">
        <div class="bg-white rounded-3xl p-10 max-w-sm w-full text-center shadow-2xl scale-90 transition-transform duration-300">
            <div id="alertIcon" class="mb-6"></div>
            <h3 id="alertTitle" class="text-2xl font-black mb-3 text-slate-900"></h3>
            <p id="alertMsg" class="text-slate-600 mb-8 leading-relaxed"></p>
            <button onclick="closeAlert()" class="w-full bg-blue-600 text-white font-bold py-4 rounded-xl hover:bg-blue-700 transition shadow-lg">關閉視窗</button>
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
            showCustomAlert('繳交成功！', '您的作業檔案「' + file.name + '」已成功傳送到伺服器。', 'check-circle-2', 'text-emerald-500');
            resetFile({ stopPropagation: () => {} });
        }

        function showCustomAlert(title, msg, icon = 'check-circle-2', iconColor = 'text-emerald-500') {
            const alert = document.getElementById('customAlert');
            document.getElementById('alertTitle').innerText = title;
            document.getElementById('alertMsg').innerText = msg;
            const iconContainer = document.getElementById('alertIcon');
            iconContainer.innerHTML = `<i data-lucide="${icon}" class="w-20 h-20 ${iconColor} mx-auto"></i>`;
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
