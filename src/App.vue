<template>

  <maApp
    :fixedSidebar="true"
    :fixedFooter="true"
  >
    <maAppHeader>
      <maAppHeaderHideSidebar></maAppHeaderHideSidebar>
      <maHeaderSearch></maHeaderSearch>
      <maHeaderNav>

        <maNotificationsDropdown
          notificationIcon="fa-bell-o"
          numberOfNotifications=10
          allNotificationsLink="#allNotifications"
        >
          <maNotificationItem
            imageURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
            content='<p> <span class="accent">Zack Alien</span> pushed new commit: <span class="accent">Fix page load performance issue</span>. </p>'
            notificationLink="#"
          >
          </maNotificationItem>

          <maNotificationItem
            imageURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
            content='<p> <span class="accent">Andy Nouman</span> deployed new version of <span class="accent">NodeJS REST Api V3</span> </p>'
            notificationLink="#"
          >
          </maNotificationItem>

          <maNotificationItem
            imageURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
            content='<p> <span class="accent">Amaya Hatsumi</span> started new task: <span class="accent">Dashboard UI design.</span>. </p>'
            notificationLink="#"
          >
          </maNotificationItem>
        </maNotificationsDropdown>

        <maNotificationsDropdown
          notificationIcon="fa-cog"
          numberOfNotifications=10
          allNotificationsLink="#allNotifications"
        >
          <maNotificationItem
            imageURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
            content='<p> <span class="accent">Zack Alien</span> pushed new commit: <span class="accent">Fix page load performance issue</span>. </p>'
            notificationLink="#"
          >
          </maNotificationItem>

          <maNotificationItem
            imageURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
            content='<p> <span class="accent">Andy Nouman</span> deployed new version of <span class="accent">NodeJS REST Api V3</span> </p>'
            notificationLink="#"
          >
          </maNotificationItem>

          <maNotificationItem
            imageURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
            content='<p> <span class="accent">Amaya Hatsumi</span> started new task: <span class="accent">Dashboard UI design.</span>. </p>'
            notificationLink="#"
          >
          </maNotificationItem>
        </maNotificationsDropdown>

        <maProfileDropdown
          name=" John Doe"
          profilePictureURL="https://avatars3.githubusercontent.com/u/3959008?v=3&s=40"
          :caret="true"
        >
          <maDropdownItem
            link="#dropdownItem1"
            icon="fa-user"
            text="Profile"
          ></maDropdownItem>
          <maDropdownItem
            link="#dropdownItem2"
            icon="fa-bell"
            text="Notifications"
          ></maDropdownItem>
          <maDropdownItem
            link="#dropdownItem3"
            icon="fa-gear"
            text="Settings"
          ></maDropdownItem>
          <maDropdownDivider></maDropdownDivider>
          <maDropdownItem
            link="#dropdownItem4"
            icon="fa-power-off"
            text="Logout"
          ></maDropdownItem>
        </maProfileDropdown>
      </maHeaderNav>
    </maAppHeader>

    <maSidebar>
      <maSidebarHeader appName="Admin"></maSidebarHeader>
      <maSidebarNav>

        <maSidebarNavDropdown
            icon="fa-th-large"
            itemText="뱃지관리"
          >
            <maSidebarNaveDropItem
            icon="fa-th-large"
            itemText="뱃지리스트"
          >
            <maSidebarNavItem
              itemText='신규등록'
            ></maSidebarNavItem>
            <maSidebarNavItem
              link='#itemslist'
              itemText='상세 페이지'
            ></maSidebarNavItem>
          </maSidebarNaveDropItem
>
        </maSidebarNavDropdown>
          <maSidebarNavDropdown
            icon="fa-th-large"
            itemText="Items Manager"
          >
            <maSidebarNavItem
              link='#itemslist'
              itemText='Items List'
            ></maSidebarNavItem>
            <maSidebarNavItem
              :active="true"
              link='#itemseditor'
              itemText='Item Editor'
            ></maSidebarNavItem>
          </maSidebarNavDropdown>
          <maSidebarNavItem
            icon='fa-th-large'
            link='#'
            itemText='운동영상관리'
          ></maSidebarNavItem>
           <maSidebarNavItem
            icon='fa-th-large'
            link='#'
            itemText='컨텐츠관리'
          ></maSidebarNavItem>
           <maSidebarNavItem
            icon='fa-th-large'
            link='#'
            itemText='CS 문의하기'
          ></maSidebarNavItem>
           <maSidebarNavItem
            icon='fa-home'
            link='#'
            itemText='관리자정보'
          ></maSidebarNavItem>
           <maSidebarNavItem
            icon='fa-home'
            link='#'
            itemText='회원정보'
          ></maSidebarNavItem>
      </maSidebarNav> 
      <maSidebarFooter></maSidebarFooter>
    </maSidebar>

    <maFooter>
      <maFooterButtons>
        <maFooterButton icon="fa-github" link="https://github.com/lulibrary"></maFooterButton>
        <maFooterButton icon="fa-twitter" link="https://twitter.com/lancasterunilib"></maFooterButton>
      </maFooterButtons>
      <maFooterAbout>
        <maFooterAboutItem>
          © Copyright Final Company, Inc. All Rights Reserved. 
대표이사 최승병 │ 사업자번호 119-86-86816 
사업장소재지 서울특별시 종로구 종로 19, 르메이에르 스포츠센터 B3층 연구소  
        </maFooterAboutItem>
        <maFooterAboutItem>
         대표전화 02-722-9502~9503 
 이메일 info@finalcompany.co.kr

        </maFooterAboutItem>
      </maFooterAbout>
    </maFooter>
    
  </maApp>

</template>

<script>
import maApp from './components/App'
import maAppHeader from './components/header/AppHeader'
import maAppHeaderHideSidebar from './components/header/HeaderHideSidebar'
import maHeaderSearch from './components/header/HeaderSearch'
import maHeaderNav from './components/header/HeaderNav'
import maNotificationsDropdown from './components/header/notifications/NotificationsDropdown'
import maNotificationItem from './components/header/notifications/NotificationItem'
import maProfileDropdown from './components/header/profile-dropdown/ProfileDropdown'
import maDropdownItem from './components/dropdown/DropdownItem'
import maDropdownDivider from './components/dropdown/DropdownDivider'
import maSidebar from './components/sidebar/Sidebar'
import maSidebarHeader from './components/sidebar/SidebarHeader'
import maSidebarNav from './components/sidebar/nav/SidebarNav'
import maSidebarNavDropdown from './components/sidebar/nav/SidebarNavDropdown'
import maSidebarNaveDropItem from './components/sidebar/nav/sidebarNaveDropItem'
import maSidebarNavItem from './components/sidebar/nav/SidebarNavItem'
import maSidebarFooter from './components/sidebar/SidebarFooter'
import maFooter from './components/footer/AppFooter'
import maFooterButtons from './components/footer/FooterButtons'
import maFooterButton from './components/footer/FooterButton'
import maFooterAbout from './components/footer/FooterAbout'
import maFooterAboutItem from './components/footer/FooterAboutItem'

export default {
  name: 'app',
  components: {
    maApp,
    maAppHeader,
    maHeaderSearch,
    maAppHeaderHideSidebar,
    maHeaderNav,
    maNotificationsDropdown,
    maNotificationItem,
    maProfileDropdown,
    maDropdownItem,
    maDropdownDivider,
    maSidebar,
    maSidebarHeader,
    maSidebarNav,
    maSidebarNavDropdown,
    maSidebarNaveDropItem,
    maSidebarNavItem,
    maSidebarFooter,
    maFooter,
    maFooterButtons,
    maFooterButton,
    maFooterAbout,
    maFooterAboutItem
  }
}
</script>
