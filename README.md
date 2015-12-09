**************************    GitHub ffmpeg-install-madeeasy    ****************************

For ffmpeg to Install and use you need to follow :

1. We intalled and tested in 'CentOs 6.6 Minimal x86_64'
2. You need internet connection and repos enabled=1
    vi /etc/yum.repos.d/CentOS-Base.repo
    #make all enabled=0 to enabled=1
3. Git installed and latest version
    yum install git
4. Make sure you installed 'hg' ie., mercurial-hgk.x86_64
        yum install hg
            or
        yum install mercurial-hgk.x86_64
5. You need to install 'FFMPEG' with 'root' Privilege


6. Make sure all the RPMs/Packages/deppendencies listed in "ffmpeg_pakg_list" are installed
7. Make sure that you installed "nasm-2.11.08" or latest *Its very important 
    (you can install by downloading nasm-2.11.08.tar.gz)
    tar xzf nasm-2.11.08.tar.gz # go into the nasm-2.11.08 directory
    ./configure
    make
    make install
8. Given two methods called...
        1)Fresh Download and install
        2)Modyfication/verify ffmpeg_sources and install 
9. 1st method will automatically hit internet and install once you run this script "ffmpeg_encoders_fresh.sh" 
        sh ffmpeg_encoders_fresh.sh


10. If it go through successfully means you can verify it by just typing "ffmpeg", by this you'll get 'ffmpeg' version and other details of 'ffmpeg' If you get any error means you need to debug...!!! ;-)
11. In 2nd method if you have "ffmpeg_sources" contents means no need of downloading the encoders required as all necessary files already in the "ffmpeg_sources" directory..., so you can run the script "ffmpeg_encoders_pre-content.sh" (this is applicable on 2nd time install/modification so you can avoid hitting intting internet everytime!)
        sh ffmpeg_encoders_pre-content.sh
12. After 2nd method you just look @ point #10 ;-)


13. After all you can make 'ffmpeg' to run in normal user mode or to root user mode by copying 'ffmpeg' binary files...
14. For #13 you just type 'which ffmpeg' and copy that binary file to the respected locations you want...like 
    cp -rf /usr/local/bin/ffmpeg /usr/bin
    cp -rf /usr/local/bin/ffmpeg /usr/sbin
    cp -rf /root/ffmpeg_build /home/'user name' #viceversa
    cp -rf /root/ffmpeg_sources /home/'user name' #viceversa
    cp -rf /root/bin /home/'user name' #viceversa
    
15. After all you can validate the 'ffmpeg' installation just by running the script "ffmpeg-install-val.sh"
        sh ffmpeg-install-val.sh
16. feel free to ask if u stuck or anything else....### naveen.mh08@gmail.com ###
17. Thank you :)

References....:
1. https://s3bubble.com/installing-ffmpeg-on-centos-6-6-in-usrlocalbin/

2. http://trac.ffmpeg.org/wiki/CompilationGuide/Centos
***********************     ffmpeg-install-madeeasy    ***************************
