<template>
    <div class="home-page">
        <section class="hero-section">
            <div class="hero-content">
                <h1>We prevent sickness with fast and painless screening solutions.</h1>
                <button class="hero-button">More</button>
            </div>
        </section>

        <section class="about-section">
            <div class="about-container">
                <img class="about-image" src="@/assets/placeholder.png" alt="About Trueeye">
                <div class="about-content">
                    <h2>About Trueeye</h2>
                    <h3>"PREVENTIVE HEALTH HERO"</h3>
                    <p>
                        True Eye is a Deep Tech Startup in the medical field co-founded by a group of doctors,
                        engineers,
                        researchers, and innovators, combining their in-depth understanding of medical and public
                        health.
                        Combined with advanced technology (deep technology) creating innovations focus on preventing
                        illnesses
                        (preventive medicine) that can be used conveniently, quickly, painlessly, and easily accessible.
                    </p>
                    <p>
                        Our technology is an artificial intelligence (AI) system for non-communicable disease (NCD)
                        screening
                        and risk assessment through retinal fundus image capturing. It is taking pictures and using AI
                        to help
                        assess health risks instead of traditional means of getting lab results from blood draws.
                    </p>
                    <div class="about-features">
                        <div class="feature">
                            <h4>FAST AND EASY</h4>
                            <p>A convenient, fast, uncomplicated examination process. The examination is completed and
                                the result is known within minutes.</p>
                        </div>
                        <div class="feature">
                            <h4>NON-INVASIVE</h4>
                            <p>Able to perform the examination safely and without pain, safe, able to examine all
                                genders and ages.</p>
                        </div>
                        <div class="feature">
                            <h4>ACCESSIBLE AND SCALABLE</h4>
                            <p>It is not necessary to use a specialist to be able to perform the examination. Scalable
                                screenings help to increase service access to a wider range.</p>
                        </div>
                        <div class="feature">
                            <h4>TRUSTED</h4>
                            <p>Through research and development from the context of Thai health from an
                                interdisciplinary group of engineers, medical professionals, hospitals, and medical
                                schools.</p>
                        </div>
                    </div>
                    <button class="about-button">More</button>
                </div>
            </div>
        </section>

    </div>
</template>

<script>
import Header from "@/components/Header_footer/Header.vue";

export default {
    components: {
        Header,
    },
};
</script>

<style scoped>

.home-page {
    display: flex;
    flex-direction: column;
    margin: 0;
    padding: 0;
}

.hero-section {
    font-family: 'Kanit', sans-serif;
    z-index: 1;
    background: url('@/assets/placeholder.png') no-repeat center center/cover;
    height: 80vh;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
}

.hero-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 700px;
    height: 700px;
    clip-path: polygon(0 0, 100% 0, 0 100%);
    background-color: #EB4648;
    z-index: 0;
}

.hero-content {
    z-index: 10;
    position: absolute;
    left: 10%;
    background: #F5F5F5;
    padding: 30px 50px;
    border-radius: 10px;
    text-align: left;
    height: 45vh;
    max-width: 600px;
}


.hero-content h1 {
    z-index: 5;
    padding-bottom: 10px;
    font-size: 2.5rem;
    margin-top: -10px;
    margin-left: -20px;
    margin-bottom: 60px;
    color: #EB4648;
}

.hero-button {
    z-index: 5;
    text-align: left;
    margin-left: -10px;
    background-color: #EB4648;
    color: white;
    padding: 10px 80px;
    border: none;
    border-radius: 30px;
    cursor: pointer;
    text-transform: uppercase;
    position: relative;
    overflow: hidden;
    transition: background-color 0.5s;
}

.hero-button::after {
    content: '\2192';
    position: absolute;
    top: 51%;
    right: 15px;
    transform: translateY(-50%);
    width: 20px;
    height: 20px;
    background-color: white;
    color: #EB4648;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    font-size: 16px;
    font-weight: 700;
    transition: transform 0.5s, background-color 0.5s, color 0.5s;
}

.hero-button:hover {
    background-color: white;
    color: #EB4648;
}

.hero-button:hover::after {
    transform: translateY(-50%) translateX(-20px);
    background-color: #EB4648;
    color: white;
    animation: arrow-slide 1s forwards;
}

@keyframes arrow-slide {
    0% {
        transform: translateY(-50%) translateX(-250px);
        background-color: #EB4648;
        color: white;
    }

    50% {
        transform: translateY(-50%) translateX(0);
        background-color: white;
        color: #EB4648;
    }

    100% {
        transform: translateY(-50%) translateX(0);
        background-color: white;
        color: #EB4648;
    }
}


.about-section {
    z-index: 1;
    background-color: #fff;
    padding: 50px 20px;
    font-family: 'Kanit', sans-serif;
    display: flex;
    justify-content: center;
}

.about-container {
    display: flex;
    padding-right: 80px;
    max-width: 1300px;
    gap: 20px;
}

.about-image {
    max-width: 400px;
    height: 700px;
    border-radius: 8px;
    box-shadow: 0 3px 8px rgba(0, 0, 0, 0.1);
}

.about-content {
    flex: 1;
}

.about-content h2 {
    font-size: 1.5rem;
    color: #333;
    margin-bottom: 8px;
}

.about-content h3 {
    font-size: 3rem;
    color: #EB4648;
    margin-bottom: 15px;
}

.about-content p {
    font-size: 1rem;
    line-height: 1.5;
    margin-bottom: 15px;
    color: #555;
}

.about-features {
    max-width: 700px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 5px;
    margin-top: 10px;
}

.feature {
    padding: 20px;
    text-align: left;
}

.feature h4 {
    font-weight: bold;
    font-size: 1.2rem;
    color: #EB4648;
    margin-bottom: 10px;
}

.feature p {
    font-weight: bold;
    font-size: 0.9rem;
    color: #666;
    line-height: 1.4;
}

.about-button {
    z-index: 5;
    text-align: left;
    margin-left: 200px;
    background-color: #EB4648;
    color: white;
    padding: 10px 80px;
    border: none;
    border-radius: 30px;
    cursor: pointer;
    text-transform: uppercase;
    position: relative;
    overflow: hidden;
    transition: background-color 0.5s;
}

.about-button::after {
    content: '\2192';
    position: absolute;
    top: 51%;
    right: 15px;
    transform: translateY(-50%);
    width: 20px;
    height: 20px;
    background-color: white;
    color: #EB4648;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    font-size: 16px;
    font-weight: 700;
    transition: transform 0.5s, background-color 0.5s, color 0.5s;
}

.about-button:hover {
    background-color: white;
    color: #EB4648;
}

.about-button:hover::after {
    transform: translateY(-50%) translateX(-20px);
    background-color: #EB4648;
    color: white;
    animation: arrow-slide 1s forwards;
}

@keyframes arrow-slide {
    0% {
        transform: translateY(-50%) translateX(-250px);
        background-color: #EB4648;
        color: white;
    }

    50% {
        transform: translateY(-50%) translateX(0);
        background-color: white;
        color: #EB4648;
    }

    100% {
        transform: translateY(-50%) translateX(0);
        background-color: white;
        color: #EB4648;
    }
}

</style>