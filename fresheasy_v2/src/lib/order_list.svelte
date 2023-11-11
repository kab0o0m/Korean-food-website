<script>
    let bulgogi_amnt = 1;
    let armystew_amnt = 3;
    let subtotal = 32;
    let total = 38;

    
    const update_subtotal = () => {
        subtotal =  (8 * bulgogi_amnt) + (8 * armystew_amnt);
        update_total()
    }

    const update_total = () => {
        if (subtotal == 0) {
            total = 0
        } else if (subtotal > 50) {
            total = subtotal;
        } else {
        total = subtotal + 6;
        }
    }

    const incr_bulgogi = () => {
        bulgogi_amnt +=1;
        update_subtotal();
        update_total();
    }

    const decr_bulgogi = () => {
        
        if (bulgogi_amnt > 0) {
            bulgogi_amnt -= 1;
        }
        update_subtotal();
        update_total();
    }

    const incr_stew = () => {
        armystew_amnt +=1;
        update_subtotal();
        update_total();
    }

    const decr_stew = () => {
        if (armystew_amnt > 0) {
            armystew_amnt -= 1;
        }
        update_subtotal();
        update_total();
    }
</script>

<div class="flex flex-col lg:pl-10 px-2 pr-2 md:pr-16 md:pl-16">
    <table class="table-auto px-16 text-center">
        <thead>
            <tr>
            <th><p class="py-2">Product</p><hr class="border-2 border-black w-full"></th>
            <th><p class="py-2">Quantity</p><hr class="border-2 border-black w-full"></th>
            <th><p class="py-2">Price</p><hr class="border-2 border-black w-full"></th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>
                    <div class="flex pr-1 py-4">
                        <img class="h-16" src="/assets/spicy_pork_bulgogi_img.png" alt="">
                        <p class="text-left p pl-4 pt-1 min-[400px]:pt-4 lg:pt-4">Spicy Pork Bulgogi</p>
                    </div>
                </td>
                <td>
                    <div class="flex justify-center px-4">
                        <button class="bg-surface-200 hover:bg-surface-300 font-xl text-surface-800 rounded-lg px-2 pb-1" on:click={decr_bulgogi}>-</button>
                        <p class="p text-center font-semibold px-4">{bulgogi_amnt}</p>
                        <button class="bg-surface-200 hover:bg-surface-300 font-xl text-surface-800 rounded-lg px-2 pb-1" on:click={incr_bulgogi}>+</button>
                    </div>
                </td>
            <td class="text-right">
                S${8 * bulgogi_amnt}.00
            </td>
            </tr>
            <tr>
            <td>
                <div class="flex pr-1 py-4">
                    <img class="h-16" src="/assets/army_stew_img.png" alt="">
                    <p class="text-left p pl-4 pt-4 lg:pt-4">Army Stew</p>
                </div>
            </td>
            <td>
                <div class="flex justify-center px-4">
                    <button class="bg-surface-200 hover:bg-surface-300 font-xl text-surface-800 rounded-lg px-2 pb-1" on:click={decr_stew}>-</button>
                    <p class="p text-center font-semibold px-4">{armystew_amnt}</p>
                    <button class="bg-surface-200 hover:bg-surface-300 font-xl text-surface-800 rounded-lg px-2 pb-1" on:click={incr_stew}>+</button>
                </div>
            </td>
            <td class="text-right">
                S${8 * armystew_amnt}.00
            </td>
            </tr>
        </tbody>
    </table>
    <hr class="mt-4 mb-8 border-2 border-black w-full">

    <div class="flex pb-8">
        <div class="w-1/2">
            <a href="mealkits" class="hover:underline">
                <div class="flex">
                    <svg xmlns="http://www.w3.org/2000/svg" class="pt-1.5 pr-2" height="1.25em" viewBox="0 0 256 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M9.4 278.6c-12.5-12.5-12.5-32.8 0-45.3l128-128c9.2-9.2 22.9-11.9 34.9-6.9s19.8 16.6 19.8 29.6l0 256c0 12.9-7.8 24.6-19.8 29.6s-25.7 2.2-34.9-6.9l-128-128z"/></svg>
                    <p>Order more...</p>
                </div>
            </a>
        </div>
        <table class="table-fixed w-1/2 text-right">
            <tr>
                <td>Subtotal:</td>
                <td>S${subtotal}.00</td>
            </tr>
            <tr>
                <td>Shipping:</td>
                <td>{(subtotal == 0 ? ("S$0.00") : (subtotal > 50 ? ("Free!") : ("$6.00")))}</td>
            </tr>
            <tr>
                <td class="font-bold">Total:</td>
                <td class="font-bold">S${total}.00</td>
            </tr>
        </table>
    </div>
    
</div>