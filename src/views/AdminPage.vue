<template>
  <div class="AdminPage" style="margin-top: -20px; padding-bottom: 50px">
    <div class="container relative" style="padding-top: 160px">
      <div
        style="
          font-size: 40px;
          font-weight: bold;
          color: var(--main-color);
          font-family: system-ui;
          text-align: center;
          margin-bottom: 25px;
        "
      >
        الإشراف
      </div>
      <div class="contain flex gap-2.5 w-100 justify-center flex-wrap">
        <router-link to="/ManageAdmins" class="box border p-2.5 hover-0">
          إدارة المشرفين
        </router-link>
        <router-link to="/TheStudents" class="box border p-2.5 hover-0">
          الطلاب
        </router-link>
        <router-link to="#" class="box border p-2.5 hover-0">
          أرباح الموقع
        </router-link>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "AdminPage",
};
</script>
<style lang="scss">
.AdminPage {
  background-image: url("../assets/background.png");
  background-size: cover;
  background-position: center top;
  background-attachment: fixed;
}
.contain > a {
  width: 32%;
  border: 1px solid var(--main-color) !important;
  border-radius: 5px;
  font-size: 22px;
  font-weight: bold;
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--main-color) !important;
  cursor: pointer;
}
@media (min-width: 1200px) {
}

@media (min-width: 768px) and (max-width: 1199px) {
}

@media (max-width: 767px) {
  .contain > a {
    width: 100% !important;
  }
}
</style>
