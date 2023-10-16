<template>
    <div class="user-card">
        <div class="card-avatar">
            <AnimatedPlaceholderVue
                height="100px"
                width="100px"
                borderRadius="50%"
            />
        </div>
        <div class="card-info">
            <AnimatedPlaceholderVue
                height="35px"
                width="200px"
            />
            <div class="summary-placeholder">
                <AnimatedPlaceholderVue
                    height="16px"
                />
                <AnimatedPlaceholderVue
                    height="16px"
                />
                <AnimatedPlaceholderVue
                    height="16px"
                />
            </div>
        </div>
    </div>
</template>

<script setup>
import AnimatedPlaceholderVue from './AnimatedPlaceholder.vue';
</script>

<style scoped>
.summary-placeholder {
    display: flex;
    flex-direction: column;
    gap: 8px;
    width: 100%;
}

</style>