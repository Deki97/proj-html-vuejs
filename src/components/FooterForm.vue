<template>
    <div class="footer-form">
        <div class="mini-title">
            Send a Message
        </div>

        <div class="heading-title">
            Get in 
            <span class="contrast-green-dark">
                Touch
            </span>
        </div>

        <div class="paragraph">
            <p>We will respond to your message as soon as possible.</p>
        </div>

        <!-- Form -->
        <form>
            <!-- Form first row (name and email) -->
            <div class="name-email d-flex justify-content-between">
                <input type="text" placeholder="Name">
                <input type="email" placeholder="Email">
            </div>
            <!-- End Form first row (name and email) -->

            <!-- Form second row (phone and info) -->
            <div class="phone-info d-flex justify-content-between">
                <input type="text" placeholder="Phone">
                
                <select name="more-info">
                    <option value="more-info">More Info</option>
                </select>
            </div>
            <!-- End Form second row (phone and info) -->

            <!-- Form Textarea -->
            <div class="message">
                <textarea name="message" cols="30" rows="5" placeholder="Message"></textarea>
            </div>
            <!-- End Form Textarea -->

            <div class="send-button">
                <button>
                    Send
                </button>
            </div>
        </form>
        <!-- End Form -->
    </div>
</template>


<script>
export default {
    name: 'FooterForm'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

.footer-form {
    .heading-title {
        color: white;
    }

    form {
        margin-top: 40px;

        div > input,
        select,
        textarea {
            color: #9a9ba2;
            background-color: #1d1d23;
            font-size: 14px;
            padding: 8px;
            border-radius: 5px;
            margin-bottom: 10px;
            border: 1px solid #1d1d23;
        }
        .name-email input,
        .phone-info input,
        .phone-info select{
            width: 50%;
            margin: 5px;
            
        }
        textarea {
            width: calc(100% - 10px);
            margin: 5px;
        }

        .more-info {
            option {
                color: #9a9ba2;
            }
        }

        button {
            background-color: $page-primary-color;
            margin: 10px 5px;
            text-transform: uppercase;
            color: white;
            font-size: 14px;
            border: 1px solid $page-primary-color;
            padding: 5px 20px;
            border-radius: 3px;
        }
    }
}
</style>