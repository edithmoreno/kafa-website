<template>
    <base-layout>
        <!--Single Column / Text-->
        <section class="contact">
            <slim-column>
                <section class="text">
                    <h1 class="title">Contacto</h1>
                    <p><span>Teléfono</span><a href="tel:(646) 135 8240">(646) 135 8240</a></p>
                    <p><span>Correo electrónico</span><a target="_blank" href="mailto:contacto@kafa.mx">contacto@kafa.mx</a> </p>
                    <p><span>Dirección</span>Calle 2da y Granada Local #9. Ensenada, Baja California. CP 22830</p>
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3388.789272573247!2d-116.6095194128525!3d31.85794906980314!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80d893bd404a0153%3A0xa49701c532dd79c9!2sKafa%20Logistics!5e0!3m2!1sen!2smx!4v1596568762935!5m2!1sen!2smx" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
                </section>
            </slim-column>
        </section>
    </base-layout>
</template>


<script>
import BaseLayout from '../layouts/BaseLayout';
export default {
  name: 'contact',
  components: { BaseLayout }, 
  metaInfo: {
    title: 'Flare Starter'
  }
}
</script>

<style lang="scss">
body {
    .contact {
        background-color: $brand-blue-5;
        padding: $gutter-xxlarge 0;
        .slim-column {
            color: white;
            iframe {
                margin-bottom: $gutter-large;
                width: 100%;
                height: rem(283px);
            }
            .title {
                color: white;
                font-size: 48px;
                font-weight: 900;
                text-transform: uppercase;
                text-shadow: 0px 2px 4px rgba(0, 0, 0, 0.51);
                margin: 0 0 16px;
            }
            p {
                    color: white;
                span {
                    font-weight: 900;
                    text-transform: uppercase;
                    font-size: rem(21px);
                    display: block;
                    margin-bottom: $gutter-small;
                }
                a {
                    color: white;
                }
            }
            ul {
                margin-bottom: $gutter;
            }
        }
    }

}
</style>