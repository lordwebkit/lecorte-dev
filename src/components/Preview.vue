<script>
export default {
    data() {
        return {
            previewList: [
                { name: 'Винная карта', link: '#' },
                { name: 'Дегустация', link: '#tasting' },
            ]
        }
    }
}
</script>
<template>
    <div class="preview">
        <div class="preview-links">
            <a v-for="previewItem in previewList" :href="previewItem.link"
                class="preview-links__link-wrapper button_gold">
                <p class="preview-links__link">{{ previewItem.name }}</p>
            </a>
        </div>
    </div>
</template>

<style scoped>
.preview {
    display: flex;
}

.preview-links {
    display: flex;
    justify-content: center;
    margin: 0 auto;
}

.preview-links__link-wrapper {
    margin-right: 30px;
}

.preview-links__link-wrapper:last-child {
    margin-right: 0px;
}


@media screen and (max-width: 1024px) {
    .button_gold {
        padding: 12px 25px;
    }

}

@media screen and (max-width: 670px) {
    .preview-links {
        flex-direction: column;
    }

    .preview-links__link-wrapper {
        margin-right: 0px;
        margin-bottom: 30px;
    }

    .preview-links__link-wrapper:last-child {
        margin: 0;
    }
}
</style>