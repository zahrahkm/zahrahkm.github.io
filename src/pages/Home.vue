<template>
  <q-page>
    <Banner :bannerText="bannerText"></Banner>

    <SeviceBox :ServiceBox="ServiceBox"></SeviceBox>

    <AboutMe :AboutMe="AboutMe" id="experience"></AboutMe>

    <Skill :Skills="Skills" id="skill"></Skill>

    <Education :education="education" ></Education>

    <MyFooter id="contact"></MyFooter>
  </q-page>
</template>

<script>
import Education from "components/EducationPart";
import SeviceBox from "components/ServiceBox";
import Skill from "components/Skill";
import AboutMe from "components/AboutMe";
import Banner from "components/Banner";
import MyFooter from "components/MyFooter";
export default {
  name: "Home",
  components:{MyFooter, Banner, AboutMe, Skill, SeviceBox, Education},
  data(){
    return{
      bannerText:"I\'m web designer and front-end developer. I'm living in Karaj, Iran. Currently, I'm a student in the master of software engineering. ",
      education:"I graduated as an IT engineering student from the Azad Islamic University of Karaj. Afterward, I found a growing urge in myself to substantiate my academic knowledge through real-world work issues. I gained a two-year experience in several web design companies to improve my skills.  Concurrently, I kept my repertoire up-to-date by taking part in online courses of Udemy. I have been becoming ready to start my Master's degree in Software engineering later on. Currently, in my second year of studying, I'm developing my Master's thesis, and as a lifetime learner, I still enjoy improving myself in innovative areas like learning other languages.",
      ServiceBox:[
        {
          title:'Front-End',
          image:'z1.png',
          text:' I did my best to stay updated and use the latest version of UI frameworks. '
        },
        {
          title:'Personality',
          image:'z2.png',
          text:' Being an ESTP personality, I enjoy learning, and I strive for it. I try to hit my best in every aspect of my life.'
        },
        {
          title:'UI&UX Design',
          image:'z3.png',
          text:" I believe creativity is the most crucial part of a design. Giving life to novel ideas in designs always amazes me."
        },
        {
          title:'IT Engineer',
          image:'z4.png',
          text:' I have always wanted to work in my major field of study and had enough related academic knowledge.'
        }
      ],
      AboutMe:[{
        title:"What I Do?",
        text:"After two-year working experience in WordPress, I found my interest in front-end developing. Hence I've started a new path learning Java Scripts and its framework Vue Js. To verbalize my ideas in designing, I've tried to reinforce the related skills with Adobe Xd and Photoshop. Nevertheless, I want to explore new fields of computer science and be a more professional programmer as time passes by."
      }]
      ,
      Skills:[
        {skill:'Html/Css', percentage: 90 },
        {skill:'JavaScript/JQuery', percentage:88},
        {skill:'Bootstrap', percentage:95},
        {skill:'Vue js', percentage:70},
        {skill:'Adobe XD', percentage:55},
        {skill:'Adobe Photoshop', percentage:65},],
    }
  }
};
</script>
<style >
  .background {
    background-size: cover;
    width: 100%;
    align-items: center;
    justify-content: center;
    height: 100%;
  }
  .marginTop{
    margin-top: 100px;
  }
  .heightsm,.education-background_heightxs{
    height: 1050px;
  }
  .heightmd,.heightxl,.heightlg{
    height: 750px;
  }
  .heightxs ,
  .education-background_heightxl{
    height: 800px;
  }
  .education-background_heightxs {
    height:1100px;
  }
  .About-background_heightmd,
  .About-background_heightlg{
    height: 490px;
  }

  element.style {
  }

  .About-background_heightxl,
  .About-background_heightxs,
  .education-background_heightlg,
  .education-background_heightmd{
    height: 550px;
  }
  .education-background_heightsm{
    height: 700px;
  }

  .light_purple{
    background-color: #ea9fe8;
  }
  .light_blue{
    background-color: #a9dde3;
  }
  .responsive {
    width: 40%;
    height: auto;
    margin-bottom: -18px;
  }

  .title_purple{
    color:#d43dcc;
  }
  .socialIcon:hover{
    color: #ea9fe8!important;
  }
  .aboutBackground-desktop{
    background-image: url('/aboutMe.jpg') !important
  }
  .aboutBackground-mobile{
    background-image: url('/aboutMe-mobile.jpg')
  }

  .educationBackground-desktop{
    background-image: url('/education.png')
  }
  .educationBackground-mobile{
     background-image: url('/education-mobile.png')!important
  }
  .contactBackground{
    background-image: url('/contactBackground.png')
  }
</style>
