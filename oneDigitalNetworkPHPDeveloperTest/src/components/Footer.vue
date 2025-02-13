<script></script>

<template>
  <div id="footerContainer">
    <div id="footer">
      <div id="topFooter">
        <div id="topFooterTextContainer">
          <div>นโยบายความเป็นส่วนตัว</div>
          <div>เงื่อนไขการใช้เว็บไซต์</div>
          <div>ตั้งค่าคุกกี้</div>
        </div>
      </div>
      <div id="bottomFooter">
        <div id="bottomFooterTextContainer">
          © 2024 binaryboutique.com. All rights reserved.
        </div>
      </div>
    </div>
  </div>
</template>

<style>
#footerContainer {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column-reverse;
}
#footer {
  height: 89.3px;
  width: 100%;

  background-color: #4285f4;
}
#topFooter {
  height: 41.53px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;

  background-color: rgba(0, 0, 0, 0.1);
}
#topFooterTextContainer {
  height: 17.8px;
  width: 425px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #ffffff;
  font-size: 12px;
}
#bottomFooter {
  height: 47.76px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;

  background-color: rgba(0, 0, 0, 0.3);
}
#bottomFooterTextContainer {
  height: 18px;
  width: 272px;

  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 12px;
  color: #FFFFFF;
}
</style>
