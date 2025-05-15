<script setup lang="ts">
import { Head } from '@inertiajs/vue3';
import AppLayout from '@/layouts/AppLayout.vue';
import { Sparkle, Check } from 'lucide-vue-next';
</script>

<template>
    <Head title="Welcome">
    </Head>

    <AppLayout>
        <div class="push-home-hero">
            <div class="push-container">
                <h1>Turn property listings into stunning videos instantly</h1>
            </div>
            <img src="/hero-phone.png" alt="" class="object-cover absolute top-0 right-0 h-full">
        </div>

        <div class="pt-28 pb-32 flex flex-col gap-30">
            <div class="push-container flex flex-col text-center items-center gap-6 px-[191px] mb-30">
                <h4>From link to video in seconds</h4>
                <p class="text-[21px]">Simply paste your property link from Rightmove or OnTheMarket, and our smart video generator does the rest—automatically and in seconds.</p>

                <div class="push-form-block pt-4 w-3/4">
                    <div class="flex w-full">
                        <input type="text" name="" id="" class="py-2.5 pl-3 w-full border-[1px] border-[#D4D4D4] rounded-l-[6px] outline-0" placeholder="Enter OnTheMarket or RightMove property URL">
                        <button class="!rounded-l-none push-btn text-nowrap">Generate Your Free Video</button>
                    </div>
                </div>

                <div class="flex gap-3">
                    <Sparkle fill="#FF7700" stroke="#FF7700"/>
                    <p>No credit card required</p>
                </div>

                <p class="text-[#6D6E71]">Example format: <br>
                    OnTheMarket: https://www.onthemarket.com/details/12345678/<br>
                    RightMove: https://www.rightmove.co.uk/properties/12345678/</p>
            </div>

            <div class="push-container text-center flex flex-col gap-16">
                <h4>How it works</h4>
                <div class="flex justify-around gap-[30px]">
                    <div class="flex flex-col gap-6 items-center w-1/3">
                        <div class="w-20 h-20 rounded-[6px] text-push-blue bg-push-blue-50 flex items-center justify-center text-[64px] font-bebas">
                            1
                        </div>

                        <div class="flex flex-col gap-2">
                            <p class="text-[20px] font-bold">Paste your link</p>
                            <p>Grab your property URL from Rightmove or OnTheMarket.</p>
                        </div>
                    </div>

                    <div class="flex flex-col gap-6 items-center w-1/3">
                        <div class="w-20 h-20 rounded-[6px] text-push-blue bg-push-blue-50 flex items-center justify-center text-[64px] font-bebas">
                            2
                        </div>

                        <div class="flex flex-col gap-2">
                            <p class="text-[20px] font-bold">One-click magic</p>
                            <p>Click generate and we'll automatically create your branded property video in moments.</p>
                        </div>
                    </div>

                    <div class="flex flex-col gap-6 items-center w-1/3">
                        <div class="w-20 h-20 rounded-[6px] text-push-blue bg-push-blue-50 flex items-center justify-center text-[64px] font-bebas">
                            3
                        </div>

                        <div class="flex flex-col gap-2">
                            <p class="text-[20px] font-bold">Share instantly</p>
                            <p>Download and share your video across social media and marketing channels effortlessly.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="pt-[205px] w-full bg-[#04103A] do-better relative overflow-hidden pb-[124px]">
            <div class="push-container">
                <div class="flex items-center">
                    <div class="relative w-1/2 flex items-center justify-center">
                        <video autoplay muted loop class="z-10">
                            <source src="/engage-video.mp4" type="video/mp4">
                        </video>

                        <img src="/effect.png" class="absolute w-[200%] z-0">
                    </div>
                    <div class="w-1/2 flex flex-col gap-6 text-white">
                        <h3 class="text-white">Ready to enhance your marketing?</h3>
                        <p>Get started now and create your first video instantly for free. No payment details required, no strings attached.</p>
                        <div class="flex flex-col gap-4">
                            <div class="flex gap-4">
                                <Check stroke="var(--color-push-blue)"/>
                                <p><strong>Save Time:</strong> Turn listings into engaging videos in seconds, no complicated tools or editing needed.</p>
                            </div>

                            <div class="flex gap-4">
                                <Check stroke="var(--color-push-blue)"/>
                                <p><strong>Professional Branding:</strong> Beautiful, branded videos that showcase your agency, impress clients, and attract buyers.</p>
                            </div>

                            <div class="flex gap-4">
                                <Check stroke="var(--color-push-blue)"/>
                                <p><strong>Effortless Simplicity:</strong> Designed for busy estate agents—no tech skills required.</p>
                            </div>

                            <div class="flex gap-4">
                                <Check stroke="var(--color-push-blue)"/>
                                <p><strong>Totally Free to Start:</strong> Generate up to x videos per month absolutely free.</p>
                            </div>

                            <div class="flex gap-4">
                                <Check stroke="var(--color-push-blue)"/>
                                <p><strong>Convenient and Accessible:</strong> Create stunning property videos from anywhere, anytime.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </AppLayout>
</template>

<style>
.do-better {
    &:before {
        content: '';
        position: absolute;
        top: -1px;
        left: 50%;
        transform: translateX(-50%);
        width: 110%;
        height: 100px;
        background-color: #fff;
        clip-path: polygon(0 0, 100% 0, 50% 100%);
    }
}
</style>
