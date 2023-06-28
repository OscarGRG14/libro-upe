<template>
    <div>
        <Navbar></Navbar>

        <main>
            <div class="container">
                <slot>
                    
                </slot>
            </div>
        </main>
    </div>
</template>

<script setup>
    useHead({
        link: [
            
            {   rel: "stylesheet",
                href: "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css",
                integrity: "sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM",
                crossorigin: "anonymous"
            },
            {
                rel: "stylesheet",
                href:"https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
            }
        ],
        script:[
            {
                src: "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"
            }
        ]   
    })
    const currentYear = new Date().getUTCFullYear();
</script>