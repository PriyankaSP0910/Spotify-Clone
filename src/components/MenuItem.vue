<script setup>
import { ref, toRefs, watchEffect } from 'vue';  //watchEffect() tracks every reactive property accessed during synchronous execution
import { useRoute } from 'vue-router';  //The useRoute package allows us to get information about the current route (the one we’re on) by getting a reference to it. To get the reference we use the useRoute method.

const route = useRoute()

const props = defineProps({           //defineProps allow us to define properties for our elements
    iconString: String,
    iconSize: Number,
    pageUrl: String,
    name: String
})
const { iconString, pageUrl, name, iconSize } = toRefs(props)    // toRef is meant to convert a property of a reactive object into a ref

let icon = ref(null)
let textIsHover = ref(false)

watchEffect(() => {
    if (route.path == pageUrl.value) {
        icon.value = iconString.value + '-active'     //if router.path==pageUrl then we set the icon to active else inactive
        textIsHover.value = true
    } else {
        icon.value = iconString.value + '-inactive'
        textIsHover.value = false
    }
})

const isHover = () => {
    if (icon.value === iconString.value + '-active') return       //if iconvalue==active return nothing

    if (icon.value === iconString.value + '-inactive') {
        icon.value = iconString.value + '-inactive-hover'
        textIsHover.value = true
    } else if (icon.value === iconString.value + '-inactive-hover') {             //if iconvalue==inactive set textIsHover to false
        icon.value = iconString.value + '-inactive'
        textIsHover.value = false
    }
}
</script>
 <template>        <!--The <template> tag itself is simply a container for all the HTML -->
   <!-- mouseover/mouseout-They trigger when the mouse pointer enters/leaves the element -->
    <li 
        class="flex items-center justify-start pb-4 cursor-pointer" 
        @mouseleave="isHover()"             
    >
        <img :width="iconSize" :src="`/images/icons/${icon}.png`">
        <!--if we are hovering over text make text white else nothing -->
        <div
            :class="textIsHover ? 'text-white ' : 'text-gray-400'"    
            class="font-semibold text-[14px] ml-4 mt-0.5"
        >
             <span :class="route.path == pageUrl ? 'text-white' : ''">{{ name }}</span>  <!--if route path = page url make text white else nothing -->
        </div>
    </li>
</template>
