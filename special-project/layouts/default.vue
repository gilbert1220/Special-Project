<script setup>
     function openNav(){
         document.querySelector('.sidebar').classList
         .toggle('left-[-15rem]');
     }
     function closeNav(){
         document.querySelector('.sidebar').classList
         .toggle('left-[-15rem]');
     }
 </script>
 
 <template>
     <div class="overflow-hidden">
        <div class="space-x-[5rem] bg-gray-300 md:hidden">
            <span @click="openNav" class="absolute bg-black top-5 left-4 cursor-pointer">
             <div class="toggle1 px-2"></div>
            </span>
            <div class="flex items-center p-2 mt-1 space-x-4">
                <div class="pl-[3rem] md:hidden"><i class="crown1"></i></div>
                <button class="flex flex-row items-center md:hidden">
                    <div>0 points1</div>
                    <div class="points1 ml-2"></div>
                </button>
                <div class="pl-[5rem]">
                    <div class="img1 md:h-[2.5rem] md:w-[2.5rem] border-2 rounded-full"></div>
                </div>
            </div>
        </div>
         <div class="sidebar bg-[#001C30] fixed top-0 bottom-0 lg:left-0 w-[15rem] md:w-[4rem] overflow-y-auto left-[-15rem]">
             <span class="flex justify-end cursor-pointer" @click="closeNav">
                <div class="close1 px-2 md:hidden"></div>
            </span>
             <div class="text-gray-100">
                 <div class="flex items-center p-2 mt-1 space-x-4">
                     <div class="img1 md:h-[2.5rem] md:w-[2.5rem] rounded-full"></div>
                     <div class="crown1 md:hidden"></div>
                     <button class="flex flex-row items-center md:hidden">
                         <div>0 points1</div>
                         <div class="points1 ml-2"></div>
                     </button>
                 </div>
                 <div class="ml-2">
                     <div class="md:hidden">Christian Gilbert Salas</div>
                     <div class="md:hidden">09512761668</div>
                 </div>
                 <div class="flex flex-col space-y-[1rem] md:space-y-[1rem] pt-[1rem]">
                     <button class="justify-start flex items-center ml-[1rem]"><p class="home mr-[1rem]"></p><i class="md:hidden">Home</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="order mr-[1rem]"></p><i class="md:hidden">Order Now</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="notif mr-[1rem]"></p><i class="md:hidden">Notifications</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="loc mr-[1rem]"></p><i class="md:hidden">Store Locator</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="faq mr-[1rem]"></p><i class="md:hidden">FAQ's</i></button>
                     <hr class="bg-gray-200 h-0.3">
                     <button class="justify-start flex items-center ml-[1rem]"><p class="order mr-[1rem]"></p><i class="md:hidden">My Order</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="user mr-[1rem]"></p><i class="md:hidden">My Accounts</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="fav mr-[1rem]"></p><i class="md:hidden">My Favorites</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="tracker mr-[1rem]"></p><i class="md:hidden">Order Tracker</i></button>
                     <button class="justify-start flex items-center ml-[1rem]"><p class="history mr-[1rem]"></p><i class="md:hidden">Order History</i></button>
                 </div>
                 <div class="pt-[11rem] md:pt-[4rem] flex justify-center">
                     <button class="bg-blue-400 h-[2rem] w-[10rem] md:w-fit rounded-lg md:rounded-full">
                        <i class="md:hidden">Logout</i><p class="logout"></p>
                    </button>
                 </div>
             </div>
         </div>
    </div>
    <div>
        <slot />
    </div>
 </template>
 
 <script>
 
 </script>
 
 <style scoped>
 
 </style>