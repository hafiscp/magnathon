<template>
    <div class="mt-20">
        <h1 class="text-[#031d44] text-7xl font-semibold">Timeline</h1>
        <hr class="mt-10 border-4 border-[#F87666] mx-[10%] w-[70%]">
    </div>
    <div class="container">
        <div class="timeline">
            <ul>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">1st Apr, 2024</h3>
                        <h2>Abstract Submission<br><span class="time">10PM onwards</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">13th Apr, 2024</h3>
                        <h2>Abstract Submission Closing<br><span class="time">12:00PM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">15th Apr, 2024</h3>
                        <h2>Shortlisted Team Release<br><span class="time">07:00PM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">17th Apr, 2024</h3>
                        <h2>Offline Registration<br><span class="time">8AM onwards</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">17th Apr, 2024</h3>
                        <h2>Inauguration<br><span class="time">9:30AM-10:30AM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">17th Apr, 2024</h3>
                        <h2>Introduction Session<br><span class="time">10:30am - 12:30pm</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">17th Apr, 2024</h3>
                        <h2>Hack Begins<br><span class="time">12:30PM onwards</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">17th Apr, 2024</h3>
                        <h2>Culturals<br><span class="time">8:00PM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">18th Apr, 2024</h3>
                        <h2>Hack Ends<br><span class="time">11:00AM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">18th Apr, 2024</h3>
                        <h2>Project Evalutaion<br><span class="time">11:00AM-12:00PM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">18th Apr, 2024</h3>
                        <h2>Result Announcement<br><span class="time">After Evalutaion</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">18th Apr, 2024</h3>
                        <h2>Project Presentation<br><span class="time">3:00PM</span></h2>
                    </div>
                </li>
                <li>
                    <div class="timeline-content">
                        <h3 class="date">18th Apr, 2024</h3>
                        <h2>Prize Distribution<br><span class="time">Tech Fest Inauguration</span></h2>
                    </div>
                </li>
            </ul>
        </div>
    </div>

</template>

<style scoped>
h1{
    font-family: 'Orbitron';
}

.container {
    min-height: 100vh;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 100px 0;
}

.timeline {
    width: 80%;
    height: auto;
    max-width: 800px;
    margin: 0 auto;
    position: relative;
}

.timeline ul {
    list-style: none;
}

.timeline ul li {
    padding: 20px;
    background-color: #166F7B;
    color: #00FFA3;
    border-radius: 10px;
    margin-bottom: 20px;
}

.timeline ul li:last-child {
    margin-bottom: 0;
}

.timeline-content h1 {
    font-weight: 500;
    font-size: 25px;
    line-height: 30px;
    margin-bottom: 10px;
}

.timeline-content p {
    font-size: 16px;
    line-height: 30px;
    font-weight: 300;
    color: #1DCC7E;
}

.timeline-content .date {
    font-size: 12px;
    font-weight: 300;
    margin-bottom: 10px;
    letter-spacing: 2px;
}

.time {
    color: #1DCC7E;
    float: right;
    font-weight: 400;
    font-size: 20px;
}

@media only screen and (min-width: 768px) {
    .timeline:before {
        content: "";
        position: absolute;
        top: 0;
        left: 50%;
        transform: translateX(-50%);
        width: 2px;
        height: 100%;
        background-color: gray;
    }

    .timeline ul li {
        width: 50%;
        position: relative;
        margin-bottom: 50px;
    }

    .timeline ul li:nth-child(odd) {
        float: left;
        clear: right;
        transform: translateX(-30px);
        border-radius: 20px 0px 20px 20px;
    }

    .timeline ul li:nth-child(even) {
        float: right;
        clear: left;
        transform: translateX(30px);
        border-radius: 0px 20px 20px 20px;
    }

    .timeline ul li::before {
        content: "";
        position: absolute;
        height: 20px;
        width: 20px;
        border-radius: 50%;
        background-color: gray;
        top: 0px;
    }

    .timeline ul li:nth-child(odd)::before {
        transform: translate(50%, -50%);
        right: -30px;
    }

    .timeline ul li:nth-child(even)::before {
        transform: translate(-50%, -50%);
        left: -30px;
    }

    .timeline-content .date {
        position: absolute;
        top: -30px;
    }

    .timeline ul li:hover::before {
        background-color: #00FFA3;
    }
}
</style>