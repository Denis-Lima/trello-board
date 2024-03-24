<template>
  <div class="p-10 h-[100vh] bg-teal-600 overflow-auto">
    <h1 class="text-4xl text-white flex items-center mb-10">
      <img width="200" class="mr-3" src="https://vueschool.io/img/logo/vueschool_logo_multicolor_negative.svg"
        alt="Vue School">
      Trello Board
    </h1>
    <TrelloBoard />
  </div>
</template>
<style>
.scrollbar {
  overflow: overlay
}

/* total width */
.scrollbar::-webkit-scrollbar {
  background-color: rgba(0, 0, 0, 0);
  width: 4px;
  height: 4px;
  z-index: 999999;
}

/* background of the scrollbar except button or resizer */
.scrollbar::-webkit-scrollbar-track {
  background-color: rgba(0, 0, 0, 0);
}

/* scrollbar itself */
.scrollbar::-webkit-scrollbar-thumb {
  background-color: rgba(0, 0, 0, 0);
  border-radius: 16px;
}

/* set button(top and bottom of the scrollbar) */
.scrollbar::-webkit-scrollbar-button {
  display: none;
}


/* scrollbar when element is hovered */
.scrollbar:hover::-webkit-scrollbar-thumb {
  background-color: #a0a0a5;
}

/* scrollbar when scrollbar is hovered */
.scrollbar::-webkit-scrollbar-thumb:hover {
  background-color: #a0a0a5;
}
</style>