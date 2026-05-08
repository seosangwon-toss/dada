```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <!-- 카톡 공유 시 보여지는 정보 세팅 -->
    <meta property="og:title" content="정다영 고객님 맞춤형 보장 분석">
    <meta property="og:description" content="서상원 어드바이저가 분석한 메리츠 The건강한 플랜 리포트입니다.">
    <meta property="og:image" content="https://i.postimg.cc/N045jnbw/1000069980.png">
    
    <title>정다영 고객님 맞춤형 보장 분석</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard.css" />
    <style>
        body {
            font-family: 'Pretendard', sans-serif;
            background-color: #f4f7fa;
            margin: 0;
            padding: 0;
            -webkit-tap-highlight-color: transparent;
        }
        .report-container {
            max-width: 480px;
            margin: 0 auto;
            background-color: #ffffff;
            min-height: 100vh;
            box-shadow: 0 0 40px rgba(0,0,0,0.08);
            padding-bottom: 50px; /* 버튼 삭제로 인한 하단 여백 축소 */
        }
        .header-gradient {
            background: linear-gradient(135deg, #002b5b 0%, #0056b3 100%);
        }
        
        /* Accordion Core Logic */
        .accordion-item {
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: 1px solid #edf2f7;
            position: relative;
        }
        
        .accordion-item.active {
            transform: scale(1.03);
            border-color: #0056b3;
            box-shadow: 0 15px 30px -10px rgba(0, 86, 179, 0.2);
            z-index: 10;
            margin-top: 12px;
            margin-bottom: 12px;
        }

        .accordion-content {
            display: grid;
            grid-template-rows: 0fr;
            transition: grid-template-rows 0.4s ease, opacity 0.3s ease;
            opacity: 0;
        }

        .active .accordion-content {
            grid-template-rows: 1fr;
            opacity: 1;
            padding-top: 16px;
            margin-top: 16px;
            border-top: 1px solid #f1f5f9;
        }

        .inner-content {
            overflow: hidden;
        }

        .chevron-icon {
            transition: transform 0.4s ease;
        }
        .active .chevron-icon {
            transform: rotate(180deg);
        }

        /* Detail List Styling */
        .detail-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 8px 0;
            font-size: 11px;
            border-bottom: 1px solid #f8fafc;
        }
        .detail-row:last-child { border-bottom: none; }
        
        .highlight-blue { color: #0056b3; font-weight: 800; }
        .highlight-purple { color: #7c3aed; font-weight: 800; }
        .highlight-cyan { color: #0891b2; font-weight: 800; }
    </style>
</head>
<body>
    <div class="report-container">
        <!-- 상단 헤더 -->
        <header class="header-gradient p-8 pb-10 text-white rounded-b-[40px] shadow-lg relative overflow-hidden">
            <div class="relative z-10">
                <!-- 토스인슈어런스 로고 -->
                <div class="mb-6 flex justify-start">
                    <div class="bg-white/10 p-3 rounded-2xl backdrop-blur-md border border-white/20 inline-flex shadow-inner">
                        <img src="https://i.postimg.cc/N045jnbw/1000069980.png" alt="토스인슈어런스 로고" class="h-10 sm:h-12 w-auto object-contain">
                    </div>
                </div>
                
                <div class="flex justify-between items-end mb-6">
                    <div>
                        <h1 class="text-2xl font-bold leading-tight mt-1">
                            정다영 고객님<br>
                            <span class="text-blue-300">메리츠 The건강한</span> 분석
                        </h1>
                        <p class="text-[10px] mt-2 opacity-60">설계번호: 32101308020260507102</p>
                    </div>
                    <div class="w-12 h-12 bg-white/10 rounded-2xl flex items-center justify-center border border-white/20">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                        </svg>
                    </div>
                </div>
                
                <div class="bg-black/20 rounded-2xl p-4 flex justify-between items-center border border-white/10 mt-2">
                    <div class="flex items-center space-x-3">
                        <div class="w-9 h-9 rounded-full bg-white/20 flex items-center justify-center text-xs font-bold">서</div>
                        <div>
                            <p class="text-[9px] opacity-60">담당 전문가</p>
                            <p class="text-xs font-bold">서상원 어드바이저</p>
                        </div>
                    </div>
                    <div class="text-right">
                        <p class="text-[9px] opacity-60">분석 기준일</p>
                        <p class="text-xs font-medium">2026.05.07</p>
                    </div>
                </div>
            </div>
        </header>

        <!-- 핵심 요약 -->
        <section class="px-6 -mt-6 mb-8 relative z-20">
            <div class="bg-white rounded-3xl p-6 shadow-xl grid grid-cols-3 gap-2 border border-slate-50">
                <div class="text-center">
                    <p class="text-[10px] text-slate-400 font-bold mb-1">납입/만기</p>
                    <p class="text-sm font-black text-slate-800">20년/100세</p>
                </div>
                <div class="text-center border-x border-slate-100">
                    <p class="text-[10px] text-slate-400 font-bold mb-1">건강등급</p>
                    <p class="text-sm font-black text-blue-600">건강고지형</p>
                </div>
                <div class="text-center">
                    <p class="text-[10px] text-slate-400 font-bold mb-1">월 총 보험료</p>
                    <p class="text-sm font-black text-blue-600">105,680원</p>
                </div>
            </div>
        </section>

        <!-- 보장 상세 리스트 -->
        <main class="px-6 space-y-4">
            <div class="flex justify-between items-end mb-4 px-1">
                <h3 class="text-sm font-black text-slate-900">항목별 상세 보장 및 보험료</h3>
                <span class="text-[9px] text-slate-400">(담보별 월납)</span>
            </div>

            <!-- 1. 암 진단비 -->
            <div class="accordion-item bg-white rounded-2xl p-5 cursor-pointer" onclick="toggleAccordion(this)">
                <div class="flex justify-between items-center">
                    <div class="flex items-center space-x-4">
                        <div class="w-10 h-10 rounded-xl bg-red-50 flex items-center justify-center text-red-500">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 18a8 8 0 100-16 8 8 0 000 16zM7 9a1 1 0 000 2h6a1 1 0 100-2H7z"/></svg>
                        </div>
                        <div>
                            <p class="text-sm font-bold text-slate-800">일반암 진단비</p>
                            <p class="text-[10px] text-slate-400">유사암 제외 모든 암 보장</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-3">
                        <div class="text-right">
                            <span class="text-lg font-black text-slate-900 block leading-tight">5,000<span class="text-xs font-medium ml-0.5">만</span></span>
                            <span class="text-[10px] font-bold text-slate-400">월 36,450원</span>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-slate-300 chevron-icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                        </svg>
                    </div>
                </div>
                <div class="accordion-content">
                    <div class="inner-content">
                        <div class="space-y-1">
                            <div class="detail-row">
                                <span class="text-slate-600">일반암 진단비</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-900 block">5,000만원</span>
                                    <span class="text-[9px] text-slate-400">31,550원</span>
                                </div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">유사암 진단비 (갑상선 등)</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-900 block">1,000만원</span>
                                    <span class="text-[9px] text-slate-400">4,900원</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 2. 암 통합치료비 -->
            <div class="accordion-item bg-white rounded-2xl p-5 cursor-pointer shadow-md shadow-purple-50" onclick="toggleAccordion(this)">
                <div class="flex justify-between items-center">
                    <div class="flex items-center space-x-4">
                        <div class="w-10 h-10 rounded-xl bg-purple-50 flex items-center justify-center text-purple-600">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg>
                        </div>
                        <div>
                            <p class="text-sm font-bold text-slate-800">암 통합치료비 (비급여)</p>
                            <p class="text-[10px] text-slate-400">항암/수술/방사선 반복 지급</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-3">
                        <div class="text-right">
                            <span class="text-lg font-black text-purple-600 block leading-tight">연 1<span class="text-xs font-medium ml-0.5">억</span></span>
                            <span class="text-[10px] font-bold text-slate-400">월 18,561원</span>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-slate-300 chevron-icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                        </svg>
                    </div>
                </div>
                <div class="accordion-content">
                    <div class="inner-content">
                        <!-- 핵심 통합보장 박스 -->
                        <div class="bg-purple-50/50 p-4 rounded-xl border border-purple-100 mb-3">
                            <div class="flex justify-between items-end mb-2 border-b border-purple-100 pb-2">
                                <p class="text-[11px] font-bold text-purple-700 flex items-center">
                                    <span class="w-1 h-3 bg-purple-400 rounded-full mr-2"></span>
                                    비급여 암 치료 통합보장
                                </p>
                                <span class="text-[9px] font-bold text-purple-500">통합 월 16,089원</span>
                            </div>
                            <div class="space-y-1 mt-2">
                                <div class="detail-row"><span class="text-slate-700">비급여 암 수술비 (회당)</span><span class="highlight-purple">2,000만원</span></div>
                                <div class="detail-row"><span class="text-slate-700">비급여 항암방사선 치료비 (연간)</span><span class="highlight-purple">2,000만원</span></div>
                                <div class="detail-row"><span class="text-slate-700">비급여 항암약물 치료비 (연간)</span><span class="highlight-purple">2,000만원</span></div>
                                <div class="detail-row mt-2 pt-2 border-t border-purple-50/50"><span class="text-slate-600">표적 / 면역 항암약물허가</span><span class="font-bold text-slate-800">각 3,000만원</span></div>
                                <div class="detail-row"><span class="text-slate-600">양성자 방사선 / 다빈치 로봇수술</span><span class="font-bold text-slate-800">3,000만 / 1,000만</span></div>
                            </div>
                        </div>
                        
                        <!-- 추가 특수치료 박스 -->
                        <div class="space-y-1 px-1">
                            <p class="text-[10px] font-bold text-slate-500 mb-1 mt-3">추가 항암/방사선 지원</p>
                            <div class="detail-row">
                                <span class="text-slate-600">중입자 방사선 치료비</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-800 block">5,000만원</span>
                                    <span class="text-[9px] text-slate-400">1,450원</span>
                                </div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">26종 항암방사선/약물치료비</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-800 block">종류별 100만원</span>
                                    <span class="text-[9px] text-slate-400">676원</span>
                                </div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">계속받는 암/기타 항암 등 (3종)</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-800 block">특약 참조</span>
                                    <span class="text-[9px] text-slate-400">346원</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 3. 2대 진단비 -->
            <div class="accordion-item bg-white rounded-2xl p-5 cursor-pointer" onclick="toggleAccordion(this)">
                <div class="flex justify-between items-center">
                    <div class="flex items-center space-x-4">
                        <div class="w-10 h-10 rounded-xl bg-blue-50 flex items-center justify-center text-blue-600">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg>
                        </div>
                        <div>
                            <p class="text-sm font-bold text-slate-800">뇌/심장질환 진단비</p>
                            <p class="text-[10px] text-slate-400">허혈성/뇌혈관 전체 보장</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-3">
                        <div class="text-right">
                            <span class="text-lg font-black text-slate-900 block leading-tight">각 2,000<span class="text-xs font-medium ml-0.5">만</span></span>
                            <span class="text-[10px] font-bold text-slate-400">월 16,731원</span>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-slate-300 chevron-icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                        </svg>
                    </div>
                </div>
                <div class="accordion-content">
                    <div class="inner-content">
                        <div class="space-y-1">
                            <div class="detail-row">
                                <span class="text-slate-600">뇌혈관질환 진단비</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-900 block">2,000만원</span>
                                    <span class="text-[9px] text-slate-400">12,300원</span>
                                </div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">허혈성심장질환 진단비</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-900 block">2,000만원</span>
                                    <span class="text-[9px] text-slate-400">3,620원</span>
                                </div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">산정특례대상 (심/뇌)</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-900 block">각 500만원</span>
                                    <span class="text-[9px] text-slate-400">505원</span>
                                </div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">특정혈전치료 (심/뇌)</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-900 block">각 2,000만원</span>
                                    <span class="text-[9px] text-slate-400">306원</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 4. 순환계 통합치료비 -->
            <div class="accordion-item bg-white rounded-2xl p-5 cursor-pointer shadow-md shadow-cyan-50" onclick="toggleAccordion(this)">
                <div class="flex justify-between items-center">
                    <div class="flex items-center space-x-4">
                        <div class="w-10 h-10 rounded-xl bg-cyan-50 flex items-center justify-center text-cyan-600">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" /></svg>
                        </div>
                        <div>
                            <p class="text-sm font-bold text-slate-800">순환계 통합치료비</p>
                            <p class="text-[10px] text-slate-400">고가 장비 및 정밀 검사 지원</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-3">
                        <div class="text-right">
                            <span class="text-lg font-black text-cyan-700 block leading-tight">5,000<span class="text-xs font-medium ml-0.5">만</span></span>
                            <span class="text-[10px] font-bold text-slate-400">월 8,272원</span>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-slate-300 chevron-icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                        </svg>
                    </div>
                </div>
                <div class="accordion-content">
                    <div class="inner-content">
                        <!-- 핵심 통합보장 박스 -->
                        <div class="bg-cyan-50/50 p-4 rounded-xl border border-cyan-100 mb-3">
                            <div class="flex justify-between items-end mb-2 border-b border-cyan-100 pb-2">
                                <p class="text-[11px] font-bold text-cyan-700 flex items-center">
                                    <span class="w-1 h-3 bg-cyan-400 rounded-full mr-2"></span>
                                    순환계 핵심 보장 내역 (연 1회)
                                </p>
                                <span class="text-[9px] font-bold text-cyan-600">통합 월 8,142원</span>
                            </div>
                            <div class="space-y-1 mt-2">
                                <div class="detail-row"><span class="text-slate-700">부분체외순환치료 (ECMO)</span><span class="highlight-cyan">2,000만원</span></div>
                                <div class="detail-row"><span class="text-slate-700">혈전용해치료</span><span class="highlight-cyan">1,000만원</span></div>
                                <div class="detail-row"><span class="text-slate-700">종합병원 중환자실 치료</span><span class="highlight-cyan">1,000만원</span></div>
                                <div class="detail-row"><span class="text-slate-700">심장/뇌 수술 (회당)</span><span class="highlight-cyan">1,000만원</span></div>
                            </div>
                        </div>
                        
                        <div class="space-y-1 px-1 mt-3">
                            <div class="detail-row">
                                <span class="text-slate-600">순환계 통합치료 생활비 (연 2회)</span>
                                <div class="text-right">
                                    <span class="font-bold text-slate-800 block">100만 / 50만원</span>
                                    <span class="text-[9px] text-slate-400">130원</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 5. 질병 수술비 -->
            <div class="accordion-item bg-white rounded-2xl p-5 cursor-pointer" onclick="toggleAccordion(this)">
                <div class="flex justify-between items-center">
                    <div class="flex items-center space-x-4">
                        <div class="w-10 h-10 rounded-xl bg-emerald-50 flex items-center justify-center text-emerald-600">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.121 14.121L19 19m-7-7l7-7m-7 7l-2.879 2.879M12 12L9.121 9.121m0 5.758L5 19m0-14l4.121 4.121" /></svg>
                        </div>
                        <div>
                            <p class="text-sm font-bold text-slate-800">질병 수술비 (1-5종)</p>
                            <p class="text-[10px] text-slate-400">수술 규모별 차등 지급</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-3">
                        <div class="text-right">
                            <span class="text-lg font-black text-slate-900 block leading-tight">최대 1,000<span class="text-xs font-medium ml-0.5">만</span></span>
                            <span class="text-[10px] font-bold text-slate-400">월 19,677원</span>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-slate-300 chevron-icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                        </svg>
                    </div>
                </div>
                <div class="accordion-content">
                    <div class="inner-content">
                        <div class="space-y-1">
                            <div class="detail-row">
                                <span class="text-slate-600">1종 (내시경 용종 등)</span>
                                <div class="text-right"><span class="font-bold text-slate-900 block">20만원</span><span class="text-[9px] text-slate-400">2,000원</span></div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">2종 (맹장 등)</span>
                                <div class="text-right"><span class="font-bold text-slate-900 block">30만원</span><span class="text-[9px] text-slate-400">1,557원</span></div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">3종 (중등도 수술)</span>
                                <div class="text-right"><span class="font-bold text-slate-900 block">100만원</span><span class="text-[9px] text-slate-400">1,620원</span></div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600">4종 (위절제 등)</span>
                                <div class="text-right"><span class="font-bold text-slate-900 block">500만원</span><span class="text-[9px] text-slate-400">800원</span></div>
                            </div>
                            <div class="detail-row">
                                <span class="text-slate-600 font-bold">5종 (심장/뇌 등 대수술)</span>
                                <div class="text-right"><span class="font-bold text-blue-600 block">1,000만원</span><span class="text-[9px] text-slate-400">13,700원</span></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 6. 기타 보장 -->
            <div class="accordion-item bg-slate-50 rounded-2xl p-5 cursor-pointer shadow-sm border border-slate-200" onclick="toggleAccordion(this)">
                <div class="flex justify-between items-center">
                    <div class="flex items-center space-x-4">
                        <div class="w-10 h-10 rounded-xl bg-slate-200 flex items-center justify-center text-slate-600">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 10h16M4 14h16M4 18h16" /></svg>
                        </div>
                        <div>
                            <p class="text-sm font-bold text-slate-800">기타 보장 내역 전체보기</p>
                            <p class="text-[10px] text-slate-500">상해 · 배상책임 등 8건</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-3">
                        <div class="text-right">
                            <span class="text-[11px] font-bold text-slate-600 block mb-0.5">상세확인</span>
                            <span class="text-[10px] font-bold text-slate-400">월 5,991원</span>
                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 text-slate-400 chevron-icon" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                        </svg>
                    </div>
                </div>
                <div class="accordion-content">
                    <div class="inner-content">
                        <div class="space-y-4 pt-2">
                            <!-- 배상책임 파트 -->
                            <div class="space-y-1">
                                <p class="text-[11px] font-bold text-slate-800 border-b border-slate-200 pb-1 mb-2">일상생활 배상책임</p>
                                <div class="detail-row">
                                    <span class="text-slate-600">가족일상생활중 배상책임(IV)</span>
                                    <div class="text-right"><span class="font-bold text-slate-900 block">1억원</span><span class="text-[9px] text-slate-400">1,870원</span></div>
                                </div>
                            </div>

                            <!-- 상해 및 입원 파트 -->
                            <div class="space-y-1">
                                <p class="text-[11px] font-bold text-slate-800 border-b border-slate-200 pb-1 mb-2">상해 보장</p>
                                <div class="detail-row">
                                    <span class="text-slate-600">상해 1~5종 수술비</span>
                                    <div class="text-right"><span class="font-bold text-slate-900 block">최대 1,000만원</span><span class="text-[9px] text-slate-400">864원</span></div>
                                </div>
                                <div class="detail-row">
                                    <span class="text-slate-600">상해 중환자실 입원일당</span>
                                    <div class="text-right"><span class="font-bold text-slate-900 block">10만원/일</span><span class="text-[9px] text-slate-400">860원</span></div>
                                </div>
                                <div class="detail-row">
                                    <span class="text-slate-600">골절 진단비 II</span>
                                    <div class="text-right"><span class="font-bold text-slate-900 block">30만원</span><span class="text-[9px] text-slate-400">2,376원</span></div>
                                </div>
                                <div class="detail-row">
                                    <span class="text-slate-600">일반상해 사망/장해</span>
                                    <div class="text-right"><span class="font-bold text-slate-900 block">각 100만원</span><span class="text-[9px] text-slate-400">21원</span></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </main>

        <!-- 푸터 메시지 (상담하기 버튼 제거) -->
        <footer class="px-6 mt-10 mb-10">
            <div class="bg-slate-900 p-8 rounded-[32px] text-white shadow-xl relative overflow-hidden">
                <div class="relative z-10">
                    <p class="text-[10px] font-bold text-blue-400 mb-2 uppercase tracking-widest">Expert's Opinion</p>
                    <h4 class="text-lg font-bold mb-4 italic">"치료 비용 리스크를<br>완벽하게 헷지한 설계입니다."</h4>
                    <p class="text-[12px] leading-relaxed opacity-80 font-light mb-2">
                        정다영 고객님, 이 플랜은 단순히 진단비만 주는 과거 방식이 아닙니다. 비급여 수술, 방사선, 약물 치료 시 각각 2천만 원씩 지원되는 통합치료비가 핵심입니다. 
                    </p>
                    <p class="text-[12px] leading-relaxed opacity-80 font-light">
                        100세까지 가장 든든한 의료 자산이 될 것입니다.
                    </p>
                </div>
            </div>
            <p class="text-center text-[10px] text-slate-400 mt-6 font-medium">Copyright © 2026 Toss Insurance Advisor Seo Sang-won</p>
        </footer>
    </div>

    <script>
        function toggleAccordion(element) {
            const isActive = element.classList.contains('active');
            
            // 모든 항목 닫기
            document.querySelectorAll('.accordion-item').forEach(item => {
                item.classList.remove('active');
            });

            // 클릭한 항목이 닫혀있었다면 열기
            if (!isActive) {
                element.classList.add('active');
                
                // 열릴 때 상단으로 부드럽게 스크롤
                setTimeout(() => {
                    const offset = 80;
                    const bodyRect = document.body.getBoundingClientRect().top;
                    const elementRect = element.getBoundingClientRect().top;
                    const elementPosition = elementRect - bodyRect;
                    const offsetPosition = elementPosition - offset;

                    window.scrollTo({
                        top: offsetPosition,
                        behavior: 'smooth'
                    });
                }, 300);
            }
        }
    </script>
</body>
</html>


```
