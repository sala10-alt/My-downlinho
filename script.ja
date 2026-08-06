const tg = window.Telegram.WebApp;
tg.ready();
tg.expand();

const user = tg.initDataUnsafe?.user;
if (user) {
  document.getElementById("userInfo").innerText =
    `مرحبًا بك ${user.first_name} 👋`;
}

tg.MainButton.setText("إرسال");
tg.MainButton.show();
tg.MainButton.onClick(() => {
  tg.sendData("تم الضغط على الزرار الرئيسي");
});

document.getElementById("mainBtn").addEventListener("click", () => {
  tg.showAlert("تم الضغط بنجاح!");
});
