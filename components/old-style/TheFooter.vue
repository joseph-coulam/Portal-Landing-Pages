<template>
    <div class="bg-gray-800 text-gray-500">
        <div class="container mx-auto">
            <div class="flex flex-col md:flex-row py-12">
                <div class="w-full md:w-1/2 px-4 mb-4">
                    <div>
                        <h2 class="text-4xl mb-2 font-bold">Terms & Conditions</h2>
                        <p>We are an information only website and aim to provide the best guides and tips but can’t guarantee to be perfect, so do note you use the information at your own risk and we can’t accept liability if things go wrong. Please email us
                            on enquiries@onlinemortgageadvisor.co.uk if you see anything that needs updating and we will do so ASAP.</p>
                        <p>The information on the site is not tailored advice to each individual reader, and as such does not constitute financial advice. All the advisors we work with are fully qualified to provide mortgage advice and work only for firms who
                            are authorised and regulated by the Financial Conduct Authority. They will offer any advice specific to you and your needs. By making an enquiry you accept that your information will be passed to one of the specialists.</p>
                    </div>
                    <div>
                        <div v-for="menuItem in footerNav" :key="menuItem.title" class="text-white py-1">
                            <a :href="menuItem.url"> {{menuItem.title}} </a>
                        </div>
                    </div>
                </div>
                <div class="w-full md:w-1/2 px-4 mb-4">
                    <div>
                        <h2 class="text-4xl mb-2 font-bold">Legal Information</h2>
                        <p>Onlinemortgageadvisor.co.uk is an information website – all of our content is written by qualified advisors from the front line, for the sole purpose of offering great, relevant, and up to date information on all things mortgages.</p>
                        <p>Online Mortgage Advisor is a trading name of FIND A MORTGAGE ONLINE LTD and is an introducer appointed representative of Finance Advice Group Ltd. We can be found on the FCA financial services register, number 697688. Find a Mortgage
                            Online Ltd is registered in England under number 8662127.</p>
                    </div>
                    <div>
                        <h2 class="text-4xl mb-2 font-bold">Follow Us</h2>
                        <div v-for="menuItem in followMenu" :key="menuItem.title" class="text-white py-1">
                            <a :href="menuItem.url"> {{menuItem.title}} </a>
                        </div>
                        <p class="my-4">© 2020 Online Mortgage Advisor. All Rights reserved.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="postcss" scoped>
p {
    @apply mb-4
}
</style>

<script>
export default {
    data() {
        return {
            footerNav: [
                { title: "About us", url: "https://www.onlinemortgageadvisor.co.uk/about-us/" },
                { title: "Careers", url: "https://www.onlinemortgageadvisor.co.uk/careers/" },
                { title: "How we use cookies", url: "https://www.onlinemortgageadvisor.co.uk/cookies/" },
                { title: "Privacy policy", url: "https://www.onlinemortgageadvisor.co.uk/privacy-policy/" },
                { title: "Complaints Procedure", url: "https://www.onlinemortgageadvisor.co.uk/contact-us/#complaints-procedure" },
                { title: "Sitemap", url: "https://www.onlinemortgageadvisor.co.uk/sitemap/" }
            ],
            followMenu: [
                { title: "Facebook", url: "https://www.facebook.com/pages/Online-Mortgage-Advisor/306800902663535/" },
                { title: "Twitter", url: "https://twitter.com/oma_mortgages/" },
                { title: "LinkedIn", url: "https://www.linkedin.com/company/online-mortgage-advisor/" }
            ]
        }
    }
}
</script>