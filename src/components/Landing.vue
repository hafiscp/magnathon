<template>
    <div id="overlay" class="text-center relative">
        <div
            class="text-6xl md:text-8xl font-sans font-bold text-palette-200 flex flex-col justify-center items-center mt-10">
            <div
                class=" flex-col lg:flex-row justify-center items-center mt-5 first-letter:font-sans hidden lg:flex">
                <div class="text-[50px] text-[#79F7FF] flex justify-center items-center"><i class="bi bi-dot"></i><span
                        class="font-extralight tracking-wider text-lg text-white">17 - 18 April, 2024</span></div>

                <div class="text-[50px] text-[#79F7FF] flex justify-center items-center"><i class="bi bi-dot"></i><span
                        class="font-extralight tracking-wider text-lg text-white">College of Engineering,
                        Vadakara</span></div>

            </div>
            <h2 class="hero"><span>Magnathon</span></h2>
            <div class="mt-5 text-xl font-sans font-bold text-[#79F7FF]">
                24 hrs National Level Hackathon
            </div>

            <div class="first-letter:font-sans text-palette-400">
                <div class="apply-button" data-hackathon-slug="magnathon2024" data-button-theme="light"
                    style="height: 44px; width: 312px"></div>

            </div>
            <!-- <div class="min-h-full px-2 flex flex-col justify-center items-center mb-20">
                <div class="grid grid-cols-2 w-[50%] sm:grid-cols-4 sm:w-[100%] items-center mx-auto">
                    <div class="flex flex-col justify-center items-center"><svg width="100%" height="100%"
                            viewBox="0 0 300 300">
                            <circle cx="150" cy="240" r="5" fill="#f26b35"></circle>
                            <circle cx="176.5279656969814" cy="236.00155252075268" r="5" fill="#f26b35"></circle>
                            <circle cx="200.69880522572598" cy="224.36148968843952" r="5" fill="#f26b35"></circle>
                            <circle cx="220.36483342212267" cy="206.11408216728603" r="5" fill="#f26b35"></circle>
                            <circle cx="233.77863737797838" cy="182.88069219297554" r="5" fill="#f26b35"></circle>
                            <circle cx="239.7483417463062" cy="156.72570842277815" r="5" fill="#f26b35"></circle>
                            <circle cx="237.74351209636413" cy="129.9731159439317" r="5" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="104.99999999999997" r="5" fill="#f26b35"></circle>
                            <circle cx="211.21554639938273" cy="84.02533153531562" r="5" fill="#f26b35"></circle>
                            <circle cx="189.04953652058023" cy="68.91280188878228" r="5" fill="#f26b35"></circle>
                            <circle cx="163.41380395585568" cy="61.00522563973843" r="5" fill="#f26b35"></circle>
                            <circle cx="136.5861960441443" cy="61.00522563973843" r="5" fill="#f26b35"></circle>
                            <circle cx="110.95046347941977" cy="68.91280188878228" r="5" fill="#f26b35"></circle>
                            <circle cx="88.78445360061724" cy="84.02533153531564" r="5" fill="#f26b35"></circle>
                            <circle cx="72.05771365940049" cy="105.00000000000004" r="5" fill="#f26b35"></circle>
                            <circle cx="62.25648790363587" cy="129.9731159439317" r="5" fill="#f26b35"></circle>
                            <circle cx="60.25165825369379" cy="156.7257084227782" r="5" fill="#f26b35"></circle>
                            <circle cx="66.22136262202163" cy="182.88069219297557" r="5" fill="#f26b35"></circle>
                            <circle cx="79.63516657787731" cy="206.114082167286" r="5" fill="#f26b35"></circle>
                            <circle cx="99.30119477427402" cy="224.36148968843955" r="5" fill="#f26b35"></circle>
                            <circle cx="123.47203430301866" cy="236.00155252075268" r="5" fill="#f26b35"></circle><text
                                x="150" y="170" text-anchor="middle" id="days" class="text-6xl font-black"
                                fill="#FFFFFF">{{
                                days }}</text>
                        </svg>
                        <h3 class="text-lg text-[#00FFA3]">days</h3>
                    </div>
                    <div class="flex flex-col justify-center items-center"><svg width="100%" height="100%"
                            viewBox="0 0 300 300">
                            <circle cx="150" cy="240" r="4" fill="#f26b35"></circle>
                            <circle cx="173.29371405922686" cy="236.93332436601617" r="4" fill="#f26b35"></circle>
                            <circle cx="195" cy="227.94228634059948" r="4" fill="#f26b35"></circle>
                            <circle cx="213.63961030678928" cy="213.63961030678928" r="4" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="195" r="4" fill="#f26b35"></circle>
                            <circle cx="236.93332436601614" cy="173.2937140592269" r="4" fill="#f26b35"></circle>
                            <circle cx="240" cy="150" r="4" fill="#f26b35"></circle>
                            <circle cx="236.93332436601617" cy="126.70628594077314" r="4" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="105.00000000000001" r="4" fill="#f26b35"></circle>
                            <circle cx="213.63961030678928" cy="86.36038969321072" r="4" fill="#f26b35"></circle>
                            <circle cx="195.00000000000003" cy="72.05771365940053" r="4" fill="#f26b35"></circle>
                            <circle cx="173.2937140592269" cy="63.06667563398386" r="4" fill="#f26b35"></circle>
                            <circle cx="150" cy="60" r="4" fill="#f26b35"></circle>
                            <circle cx="126.70628594077317" cy="63.06667563398385" r="4" fill="#f26b35"></circle>
                            <circle cx="105.00000000000003" cy="72.05771365940052" r="4" fill="#f26b35"></circle>
                            <circle cx="86.36038969321075" cy="86.36038969321069" r="4" fill="#f26b35"></circle>
                            <circle cx="72.05771365940053" cy="104.99999999999997" r="4" fill="#f26b35"></circle>
                            <circle cx="63.06667563398388" cy="126.70628594077307" r="4" fill="#f26b35"></circle>
                            <circle cx="60" cy="150" r="4" fill="#f26b35"></circle>
                            <circle cx="63.06667563398385" cy="173.29371405922683" r="4" fill="#f26b35"></circle>
                            <circle cx="72.05771365940049" cy="194.99999999999994" r="4" fill="#f26b35"></circle>
                            <circle cx="86.3603896932107" cy="213.63961030678928" r="4" fill="#f26b35"></circle>
                            <circle cx="104.99999999999996" cy="227.94228634059945" r="4" fill="#f26b35"></circle>
                            <circle cx="126.70628594077306" cy="236.9333243660161" r="4" fill="#f26b35"></circle><text
                                x="150" y="170" text-anchor="middle" id="hours" class="text-6xl font-black"
                                fill="#FFFFFF">{{ hours }}</text>
                        </svg>
                        <h3 class="text-lg text-[#00FFA3]">hours</h3>
                    </div>
                    <div class="flex flex-col justify-center items-center"><svg width="100%" height="100%"
                            viewBox="0 0 300 300">
                            <circle cx="150" cy="240" r="2" fill="#f26b35"></circle>
                            <circle cx="159.4075616940888" cy="239.5069705831446" r="2" fill="#f26b35"></circle>
                            <circle cx="168.71205217359835" cy="238.03328406604248" r="2" fill="#f26b35"></circle>
                            <circle cx="177.81152949374527" cy="235.59508646656383" r="2" fill="#f26b35"></circle>
                            <circle cx="186.60629787682203" cy="232.21909118783407" r="2" fill="#f26b35"></circle>
                            <circle cx="195" cy="227.94228634059948" r="2" fill="#f26b35"></circle>
                            <circle cx="202.90067270632258" cy="222.81152949374527" r="2" fill="#f26b35"></circle>
                            <circle cx="210.22175457229724" cy="216.88303429296548" r="2" fill="#f26b35"></circle>
                            <circle cx="216.88303429296548" cy="210.22175457229724" r="2" fill="#f26b35"></circle>
                            <circle cx="222.81152949374527" cy="202.90067270632258" r="2" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="195" r="2" fill="#f26b35"></circle>
                            <circle cx="232.21909118783407" cy="186.60629787682203" r="2" fill="#f26b35"></circle>
                            <circle cx="235.59508646656383" cy="177.81152949374527" r="2" fill="#f26b35"></circle>
                            <circle cx="238.03328406604248" cy="168.71205217359835" r="2" fill="#f26b35"></circle>
                            <circle cx="239.5069705831446" cy="159.40756169408883" r="2" fill="#f26b35"></circle>
                            <circle cx="240" cy="150" r="2" fill="#f26b35"></circle>
                            <circle cx="239.5069705831446" cy="140.5924383059112" r="2" fill="#f26b35"></circle>
                            <circle cx="238.0332840660425" cy="131.28794782640168" r="2" fill="#f26b35"></circle>
                            <circle cx="235.59508646656383" cy="122.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="232.21909118783407" cy="113.39370212317799" r="2" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="105.00000000000001" r="2" fill="#f26b35"></circle>
                            <circle cx="222.81152949374527" cy="97.09932729367742" r="2" fill="#f26b35"></circle>
                            <circle cx="216.8830342929655" cy="89.77824542770279" r="2" fill="#f26b35"></circle>
                            <circle cx="210.22175457229724" cy="83.11696570703452" r="2" fill="#f26b35"></circle>
                            <circle cx="202.90067270632258" cy="77.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="195.00000000000003" cy="72.05771365940053" r="2" fill="#f26b35"></circle>
                            <circle cx="186.60629787682203" cy="67.78090881216592" r="2" fill="#f26b35"></circle>
                            <circle cx="177.81152949374527" cy="64.40491353343619" r="2" fill="#f26b35"></circle>
                            <circle cx="168.71205217359838" cy="61.9667159339575" r="2" fill="#f26b35"></circle>
                            <circle cx="159.40756169408883" cy="60.49302941685541" r="2" fill="#f26b35"></circle>
                            <circle cx="150" cy="60" r="2" fill="#f26b35"></circle>
                            <circle cx="140.59243830591123" cy="60.49302941685539" r="2" fill="#f26b35"></circle>
                            <circle cx="131.28794782640168" cy="61.96671593395749" r="2" fill="#f26b35"></circle>
                            <circle cx="122.18847050625473" cy="64.40491353343617" r="2" fill="#f26b35"></circle>
                            <circle cx="113.393702123178" cy="67.7809088121659" r="2" fill="#f26b35"></circle>
                            <circle cx="105.00000000000003" cy="72.05771365940052" r="2" fill="#f26b35"></circle>
                            <circle cx="97.09932729367742" cy="77.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="89.77824542770279" cy="83.1169657070345" r="2" fill="#f26b35"></circle>
                            <circle cx="83.11696570703454" cy="89.77824542770276" r="2" fill="#f26b35"></circle>
                            <circle cx="77.18847050625475" cy="97.0993272936774" r="2" fill="#f26b35"></circle>
                            <circle cx="72.05771365940053" cy="104.99999999999997" r="2" fill="#f26b35"></circle>
                            <circle cx="67.78090881216595" cy="113.39370212317792" r="2" fill="#f26b35"></circle>
                            <circle cx="64.40491353343619" cy="122.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="61.9667159339575" cy="131.28794782640162" r="2" fill="#f26b35"></circle>
                            <circle cx="60.49302941685541" cy="140.59243830591112" r="2" fill="#f26b35"></circle>
                            <circle cx="60" cy="150" r="2" fill="#f26b35"></circle>
                            <circle cx="60.49302941685539" cy="159.40756169408877" r="2" fill="#f26b35"></circle>
                            <circle cx="61.966715933957474" cy="168.71205217359827" r="2" fill="#f26b35"></circle>
                            <circle cx="64.40491353343617" cy="177.81152949374524" r="2" fill="#f26b35"></circle>
                            <circle cx="67.7809088121659" cy="186.606297876822" r="2" fill="#f26b35"></circle>
                            <circle cx="72.05771365940049" cy="194.99999999999994" r="2" fill="#f26b35"></circle>
                            <circle cx="77.18847050625472" cy="202.90067270632258" r="2" fill="#f26b35"></circle>
                            <circle cx="83.11696570703448" cy="210.22175457229721" r="2" fill="#f26b35"></circle>
                            <circle cx="89.7782454277027" cy="216.88303429296542" r="2" fill="#f26b35"></circle>
                            <circle cx="97.0993272936774" cy="222.81152949374524" r="2" fill="#f26b35"></circle>
                            <circle cx="104.99999999999996" cy="227.94228634059945" r="2" fill="#f26b35"></circle>
                            <circle cx="113.39370212317792" cy="232.21909118783407" r="2" fill="#f26b35"></circle>
                            <circle cx="122.18847050625472" cy="235.59508646656383" r="2" fill="#f26b35"></circle>
                            <circle cx="131.28794782640162" cy="238.03328406604248" r="2" fill="#f26b35"></circle>
                            <circle cx="140.59243830591112" cy="239.5069705831446" r="2" fill="#f26b35"></circle><text
                                x="150" y="170" text-anchor="middle" id="minutes" class="text-6xl font-black"
                                fill="#FFFFFF">{{ minutes }}</text>
                        </svg>
                        <h3 class="text-lg text-[#00FFA3]">minutes</h3>
                    </div>
                    <div class="flex flex-col justify-center items-center"><svg width="100%" height="100%"
                            viewBox="0 0 300 300">
                            <circle cx="150" cy="240" r="2" fill="#f26b35"></circle>
                            <circle cx="159.4075616940888" cy="239.5069705831446" r="2" fill="#f26b35"></circle>
                            <circle cx="168.71205217359835" cy="238.03328406604248" r="2" fill="#f26b35"></circle>
                            <circle cx="177.81152949374527" cy="235.59508646656383" r="2" fill="#f26b35"></circle>
                            <circle cx="186.60629787682203" cy="232.21909118783407" r="2" fill="#f26b35"></circle>
                            <circle cx="195" cy="227.94228634059948" r="2" fill="#f26b35"></circle>
                            <circle cx="202.90067270632258" cy="222.81152949374527" r="2" fill="#f26b35"></circle>
                            <circle cx="210.22175457229724" cy="216.88303429296548" r="2" fill="#f26b35"></circle>
                            <circle cx="216.88303429296548" cy="210.22175457229724" r="2" fill="#f26b35"></circle>
                            <circle cx="222.81152949374527" cy="202.90067270632258" r="2" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="195" r="2" fill="#f26b35"></circle>
                            <circle cx="232.21909118783407" cy="186.60629787682203" r="2" fill="#f26b35"></circle>
                            <circle cx="235.59508646656383" cy="177.81152949374527" r="2" fill="#f26b35"></circle>
                            <circle cx="238.03328406604248" cy="168.71205217359835" r="2" fill="#f26b35"></circle>
                            <circle cx="239.5069705831446" cy="159.40756169408883" r="2" fill="#f26b35"></circle>
                            <circle cx="240" cy="150" r="2" fill="#f26b35"></circle>
                            <circle cx="239.5069705831446" cy="140.5924383059112" r="2" fill="#f26b35"></circle>
                            <circle cx="238.0332840660425" cy="131.28794782640168" r="2" fill="#f26b35"></circle>
                            <circle cx="235.59508646656383" cy="122.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="232.21909118783407" cy="113.39370212317799" r="2" fill="#f26b35"></circle>
                            <circle cx="227.94228634059948" cy="105.00000000000001" r="2" fill="#f26b35"></circle>
                            <circle cx="222.81152949374527" cy="97.09932729367742" r="2" fill="#f26b35"></circle>
                            <circle cx="216.8830342929655" cy="89.77824542770279" r="2" fill="#f26b35"></circle>
                            <circle cx="210.22175457229724" cy="83.11696570703452" r="2" fill="#f26b35"></circle>
                            <circle cx="202.90067270632258" cy="77.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="195.00000000000003" cy="72.05771365940053" r="2" fill="#f26b35"></circle>
                            <circle cx="186.60629787682203" cy="67.78090881216592" r="2" fill="#f26b35"></circle>
                            <circle cx="177.81152949374527" cy="64.40491353343619" r="2" fill="#f26b35"></circle>
                            <circle cx="168.71205217359838" cy="61.9667159339575" r="2" fill="#f26b35"></circle>
                            <circle cx="159.40756169408883" cy="60.49302941685541" r="2" fill="#f26b35"></circle>
                            <circle cx="150" cy="60" r="2" fill="#f26b35"></circle>
                            <circle cx="140.59243830591123" cy="60.49302941685539" r="2" fill="#f26b35"></circle>
                            <circle cx="131.28794782640168" cy="61.96671593395749" r="2" fill="#f26b35"></circle>
                            <circle cx="122.18847050625473" cy="64.40491353343617" r="2" fill="#f26b35"></circle>
                            <circle cx="113.393702123178" cy="67.7809088121659" r="2" fill="#f26b35"></circle>
                            <circle cx="105.00000000000003" cy="72.05771365940052" r="2" fill="#f26b35"></circle>
                            <circle cx="97.09932729367742" cy="77.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="89.77824542770279" cy="83.1169657070345" r="2" fill="#f26b35"></circle>
                            <circle cx="83.11696570703454" cy="89.77824542770276" r="2" fill="#f26b35"></circle>
                            <circle cx="77.18847050625475" cy="97.0993272936774" r="2" fill="#f26b35"></circle>
                            <circle cx="72.05771365940053" cy="104.99999999999997" r="2" fill="#f26b35"></circle>
                            <circle cx="67.78090881216595" cy="113.39370212317792" r="2" fill="#f26b35"></circle>
                            <circle cx="64.40491353343619" cy="122.18847050625473" r="2" fill="#f26b35"></circle>
                            <circle cx="61.9667159339575" cy="131.28794782640162" r="2" fill="#f26b35"></circle>
                            <circle cx="60.49302941685541" cy="140.59243830591112" r="2" fill="#f26b35"></circle>
                            <circle cx="60" cy="150" r="2" fill="#f26b35"></circle>
                            <circle cx="60.49302941685539" cy="159.40756169408877" r="2" fill="#f26b35"></circle>
                            <circle cx="61.966715933957474" cy="168.71205217359827" r="2" fill="#f26b35"></circle>
                            <circle cx="64.40491353343617" cy="177.81152949374524" r="2" fill="#f26b35"></circle>
                            <circle cx="67.7809088121659" cy="186.606297876822" r="2" fill="#f26b35"></circle>
                            <circle cx="72.05771365940049" cy="194.99999999999994" r="2" fill="#f26b35"></circle>
                            <circle cx="77.18847050625472" cy="202.90067270632258" r="2" fill="#f26b35"></circle>
                            <circle cx="83.11696570703448" cy="210.22175457229721" r="2" fill="#f26b35"></circle>
                            <circle cx="89.7782454277027" cy="216.88303429296542" r="2" fill="#f26b35"></circle>
                            <circle cx="97.0993272936774" cy="222.81152949374524" r="2" fill="#f26b35"></circle>
                            <circle cx="104.99999999999996" cy="227.94228634059945" r="2" fill="#f26b35"></circle>
                            <circle cx="113.39370212317792" cy="232.21909118783407" r="2" fill="#f26b35"></circle>
                            <circle cx="122.18847050625472" cy="235.59508646656383" r="2" fill="#f26b35"></circle>
                            <circle cx="131.28794782640162" cy="238.03328406604248" r="2" fill="#f26b35"></circle>
                            <circle cx="140.59243830591112" cy="239.5069705831446" r="2" fill="#f26b35"></circle><text
                                x="150" y="170" text-anchor="middle" id="seconds" class="text-6xl font-black"
                                fill="#FFFFFF">{{ seconds }}</text>
                        </svg>
                        <h3 class="text-lg text-[#00FFA3]">seconds</h3>
                    </div>
                </div>
            </div> -->
        </div>
    </div>
</template>

<style scoped>
.hero {
    font-size: clamp(40px, 10vw, 100px);
    line-height: 1;
    display: inline-block;
    color: #fff;
    z-index: 2;
    letter-spacing: 2px;

    /* Bright things in dark environments usually cast that light, giving off a glow */
    filter: drop-shadow(0 1px 3px);
}


.layers {
    position: relative;
}

.layers::before,
.layers::after {
    content: attr(data-text);
    position: absolute;
    width: 110%;
    z-index: -1;
}

.layers::before {
    top: 10px;
    left: 15px;
    color: #e0287d;
}

.layers::after {
    top: 5px;
    left: -10px;
    color: #1bc7fb;
}

.single-path {
    clip-path: polygon(0% 12%,
            53% 12%,
            53% 26%,
            25% 26%,
            25% 86%,
            31% 86%,
            31% 0%,
            53% 0%,
            53% 84%,
            92% 84%,
            92% 82%,
            70% 82%,
            70% 29%,
            78% 29%,
            78% 65%,
            69% 65%,
            69% 66%,
            77% 66%,
            77% 45%,
            85% 45%,
            85% 26%,
            97% 26%,
            97% 28%,
            84% 28%,
            84% 34%,
            54% 34%,
            54% 89%,
            30% 89%,
            30% 58%,
            83% 58%,
            83% 5%,
            68% 5%,
            68% 36%,
            62% 36%,
            62% 1%,
            12% 1%,
            12% 34%,
            60% 34%,
            60% 57%,
            98% 57%,
            98% 83%,
            1% 83%,
            1% 53%,
            91% 53%,
            91% 84%,
            8% 84%,
            8% 83%,
            4% 83%);
}

.paths {
    animation: paths 6s step-end infinite;
}

@keyframes paths {
    0% {
        clip-path: polygon(0% 43%,
                83% 43%,
                83% 22%,
                23% 22%,
                23% 24%,
                91% 24%,
                91% 26%,
                18% 26%,
                18% 83%,
                29% 83%,
                29% 17%,
                41% 17%,
                41% 39%,
                18% 39%,
                18% 82%,
                54% 82%,
                54% 88%,
                19% 88%,
                19% 4%,
                39% 4%,
                39% 14%,
                76% 14%,
                76% 52%,
                23% 52%,
                23% 35%,
                19% 35%,
                19% 8%,
                36% 8%,
                36% 31%,
                73% 31%,
                73% 16%,
                1% 16%,
                1% 56%,
                50% 56%,
                50% 8%);
    }

    5% {
        clip-path: polygon(0% 29%,
                44% 29%,
                44% 83%,
                94% 83%,
                94% 56%,
                11% 56%,
                11% 64%,
                94% 64%,
                94% 70%,
                88% 70%,
                88% 32%,
                18% 32%,
                18% 96%,
                10% 96%,
                10% 62%,
                9% 62%,
                9% 84%,
                68% 84%,
                68% 50%,
                52% 50%,
                52% 55%,
                35% 55%,
                35% 87%,
                25% 87%,
                25% 39%,
                15% 39%,
                15% 88%,
                52% 88%);
    }

    30% {
        clip-path: polygon(0% 53%,
                93% 53%,
                93% 62%,
                68% 62%,
                68% 37%,
                97% 37%,
                97% 89%,
                13% 89%,
                13% 45%,
                51% 45%,
                51% 88%,
                17% 88%,
                17% 54%,
                81% 54%,
                81% 75%,
                79% 75%,
                79% 76%,
                38% 76%,
                38% 28%,
                61% 28%,
                61% 12%,
                55% 12%,
                55% 62%,
                68% 62%,
                68% 51%,
                0% 51%,
                0% 92%,
                63% 92%,
                63% 4%,
                65% 4%);
    }

    45% {
        clip-path: polygon(0% 33%,
                2% 33%,
                2% 69%,
                58% 69%,
                58% 94%,
                55% 94%,
                55% 25%,
                33% 25%,
                33% 85%,
                16% 85%,
                16% 19%,
                5% 19%,
                5% 20%,
                79% 20%,
                79% 96%,
                93% 96%,
                93% 50%,
                5% 50%,
                5% 74%,
                55% 74%,
                55% 57%,
                96% 57%,
                96% 59%,
                87% 59%,
                87% 65%,
                82% 65%,
                82% 39%,
                63% 39%,
                63% 92%,
                4% 92%,
                4% 36%,
                24% 36%,
                24% 70%,
                1% 70%,
                1% 43%,
                15% 43%,
                15% 28%,
                23% 28%,
                23% 71%,
                90% 71%,
                90% 86%,
                97% 86%,
                97% 1%,
                60% 1%,
                60% 67%,
                71% 67%,
                71% 91%,
                17% 91%,
                17% 14%,
                39% 14%,
                39% 30%,
                58% 30%,
                58% 11%,
                52% 11%,
                52% 83%,
                68% 83%);
    }

    76% {
        clip-path: polygon(0% 26%,
                15% 26%,
                15% 73%,
                72% 73%,
                72% 70%,
                77% 70%,
                77% 75%,
                8% 75%,
                8% 42%,
                4% 42%,
                4% 61%,
                17% 61%,
                17% 12%,
                26% 12%,
                26% 63%,
                73% 63%,
                73% 43%,
                90% 43%,
                90% 67%,
                50% 67%,
                50% 41%,
                42% 41%,
                42% 46%,
                50% 46%,
                50% 84%,
                96% 84%,
                96% 78%,
                49% 78%,
                49% 25%,
                63% 25%,
                63% 14%);
    }

    90% {
        clip-path: polygon(0% 41%,
                13% 41%,
                13% 6%,
                87% 6%,
                87% 93%,
                10% 93%,
                10% 13%,
                89% 13%,
                89% 6%,
                3% 6%,
                3% 8%,
                16% 8%,
                16% 79%,
                0% 79%,
                0% 99%,
                92% 99%,
                92% 90%,
                5% 90%,
                5% 60%,
                0% 60%,
                0% 48%,
                89% 48%,
                89% 13%,
                80% 13%,
                80% 43%,
                95% 43%,
                95% 19%,
                80% 19%,
                80% 85%,
                38% 85%,
                38% 62%);
    }

    1%,
    7%,
    33%,
    47%,
    78%,
    93% {
        clip-path: none;
    }
}

.movement {
    /* Normally this position would be absolute & on the layers, set to relative here so we can see it on the div */
    position: relative;
    animation: movement 200s step-end infinite;
}

@keyframes movement {
    0% {
        top: 0px;
        left: -20px;
    }

    15% {
        top: 10px;
        left: 10px;
    }

    60% {
        top: 5px;
        left: -10px;
    }

    75% {
        top: -5px;
        left: 20px;
    }

    100% {
        top: 10px;
        left: 5px;
    }
}

.opacity {
    animation: opacity 5s step-end infinite;
}

@keyframes opacity {
    0% {
        opacity: 0.1;
    }

    5% {
        opacity: 0.7;
    }

    30% {
        opacity: 0.4;
    }

    45% {
        opacity: 0.6;
    }

    76% {
        opacity: 0.4;
    }

    90% {
        opacity: 0.8;
    }

    1%,
    7%,
    33%,
    47%,
    78%,
    93% {
        opacity: 0;
    }
}

.font {
    animation: font 7s step-end infinite;
}

@keyframes font {
    0% {
        font-weight: 100;
        color: #e0287d;
        filter: blur(3px);
    }

    20% {
        font-weight: 500;
        color: #fff;
        filter: blur(0);
    }

    50% {
        font-weight: 300;
        color: #1bc7fb;
        filter: blur(2px);
    }

    60% {
        font-weight: 700;
        color: #fff;
        filter: blur(0);
    }

    90% {
        font-weight: 500;
        color: #e0287d;
        filter: blur(6px);
    }
}

.glitch span {
    animation: paths 5s step-end infinite;
}

.glitch::before {
    animation: paths 5s step-end infinite, opacity 5s step-end infinite,
        font 8s step-end infinite, movement 10s step-end infinite;
}

.glitch::after {
    animation: paths 5s step-end infinite, opacity 5s step-end infinite,
        font 7s step-end infinite, movement 8s step-end infinite;
}
</style>

<script setup>
import { ref, onMounted } from 'vue';

const days = ref(0);
const hours = ref(0);
const minutes = ref(0);
const seconds = ref(0);
const countDownDate = new Date("Apr 17, 2024 09:00:00").getTime();

const updateCountdown = () => {
    let now = new Date().getTime();
    let distance = countDownDate - now;

    days.value = Math.floor(distance / (1000 * 60 * 60 * 24));
    hours.value = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    minutes.value = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    seconds.value = Math.floor((distance % (1000 * 60)) / 1000);
};

onMounted(() => {
    updateCountdown();
    setInterval(updateCountdown, 1000);
});
</script>