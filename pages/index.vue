<template>
    <div class="bg-primary w-full">
        <div class="flex justify-center relative top-9 gap-4 lg:gap-8">
            <button type="button" class="rounded-2xl w-28 bg-primary  text-white shadow-md text-center">
                <img src="~/assets/img/airplane.jpg" alt="airplane" class="rounded-t-2xl w-full h-24 object-cover" />
                <div class="p-2 text-sm">Penerbangan</div>
            </button>
            <button type="button" class="rounded-2xl w-28 bg-white shadow-md text-center">
                <img src="~/assets/img/hotel.jpg" alt="airplane" class="rounded-t-2xl w-full h-24 object-cover" />
                <div class="p-2 text-sm">Hotel</div>
            </button>
        </div>
    </div>

    <form class="container pt-20 px-3">
        <div class="flex gap-3">
            <button type="button" class="bg-primary text-white px-6 py-3 rounded-md">
                Sekali Jalan
            </button>
            <button type="button" class="bg-gray-200 px-6 py-3 rounded-md">
                Pulang Pergi
            </button>
        </div>

        <div class="mt-4 grid gap-3 lg:gap-4 grid-cols-2 sm:grid-cols-2 md:grid-cols-4">
            <div>
                <label for="from" class="text-[10px] lg:text-sm">Dari</label>
                <input type="text" placeholder="Pilih Kota atau Bandara"
                    class="text-gray-500 bg-no-repeat text-sm bg-[center_right_4px] w-full py-2 pl-2 pr-7 border border-gray-400 rounded-md bg-[length:24px_24px] bg-[url('~/assets/icon/location_map_marker_icon.svg')]" />
            </div>
            <div>
                <label for="to" class="text-[10px] lg:text-sm">Tujuan</label>
                <input type="text" placeholder="Pilih Kota atau Bandara"
                    class="text-gray-500 bg-no-repeat text-sm bg-[center_right_4px] w-full py-2 pl-2 pr-7 border border-gray-400 rounded-md bg-[length:24px_24px] bg-[url('~/assets/icon/location_map_marker_icon.svg')]" />
            </div>
            <div>
                <label for="start" class="text-[10px] lg:text-sm">Tanggal Keberangkatan</label>
                <input type="text" placeholder="9/1/2023"
                    class="text-gray-500 bg-no-repeat text-sm bg-[center_right_4px] w-full py-2 pl-2 pr-7 border border-gray-400 rounded-md bg-[length:24px_24px] bg-[url('~/assets/icon/calendar_events_schedule_icon.svg')]" />
            </div>
            <div>
                <label for="end" class="text-[10px] lg:text-sm">Tanggal Kepulangan</label>
                <input type="text" placeholder="9/1/2023"
                    class="text-gray-500 bg-no-repeat text-sm bg-[center_right_4px] w-full py-2 pl-2 pr-7 border border-gray-400 rounded-md bg-[length:24px_24px] bg-[url('~/assets/icon/calendar_events_schedule_icon.svg')]" />
            </div>
        </div>

        <div class="mt-4 grid gap-3 lg:gap-4 grid-cols-2 sm:grid-cols-2 md:grid-cols-4">
            <div>
                <label for="class" class="text-[10px] lg:text-sm">Kelas</label>
                <select
                    class="block text-gray-500 w-full text-sm bg-[length:24px_24px] bg-no-repeat bg-[center_right_4px] bg-white border border-gray-400 py-2 pl-2 pr-7 rounded-md appearance-none bg-[url('~/assets/icon/arrow_bottom_down_icon.svg')]">
                    <option>
                        Economy
                    </option>
                    <option>
                        Business
                    </option>
                    <option>
                        First
                    </option>
                </select>
            </div>
            <div>
                <label for="airlane" class="text-[10px] lg:text-sm">Maskapai</label>
                <input type="text" placeholder="Tampilkan semua"
                    class="text-gray-500 bg-no-repeat text-sm bg-[center_right_4px] w-full py-2 pl-2 pr-7 border border-gray-400 rounded-md" />
            </div>
            <div class="col-span-2 grid gap-3 lg:gap-4 grid-cols-3">
                <div>
                    <label for="adult" class="text-[10px] lg:text-sm">Dewasa Usia 12+</label>
                    <div class="flex">
                        <button type="button"
                            class="rounded-l-md border border-gray-400 flex items-center px-3 sm:px-5 md:px-3 lg:px-5 text-xl">&minus;</button>
                        <div
                            class="text-gray-500 text-center bg-no-repeat text-sm bg-[center_right_4px] w-full p-2 border-y border-gray-400">
                            1
                        </div>
                        <button type="button"
                            class="rounded-r-md border border-gray-400 flex items-center px-3 sm:px-5 md:px-3 lg:px-5 text-xl">&plus;</button>
                    </div>
                </div>
                <div>
                    <label for="child" class="text-[10px] lg:text-sm">Anak Usia 2-11 tahun</label>
                    <div class="flex">
                        <button type="button"
                            class="rounded-l-md border border-gray-400 flex items-center px-3 sm:px-5 md:px-3 lg:px-5 text-xl">&minus;</button>
                        <div
                            class="text-gray-500 text-center bg-no-repeat text-sm bg-[center_right_4px] w-full p-2 border-y border-gray-400">
                            1
                        </div>
                        <button type="button"
                            class="rounded-r-md border border-gray-400 flex items-center px-3 sm:px-5 md:px-3 lg:px-5 text-xl">&plus;</button>
                    </div>
                </div>
                <div>
                    <label for="baby" class="text-[10px] lg:text-sm">Bayi di bawah 2 tahun</label>
                    <div class="flex">
                        <button type="button"
                            class="rounded-l-md border border-gray-400 flex items-center px-3 sm:px-5 md:px-3 lg:px-5 text-xl">&minus;</button>
                        <div
                            class="text-gray-500 text-center bg-no-repeat text-sm bg-[center_right_4px] w-full p-2 border-y border-gray-400">
                            1
                        </div>
                        <button type="button"
                            class="rounded-r-md border border-gray-400 flex items-center px-3 sm:px-5 md:px-3 lg:px-5 text-xl">&plus;</button>
                    </div>
                </div>
            </div>
        </div>

        <div class="mt-7 md:mt-10 flex md:justify-end">
            <button type="submit" class="bg-primary block md:inline-block w-full md:w-auto text-white px-6 py-3 rounded-md">
                Cari Penerbangan
            </button>
        </div>
    </form>
</template>