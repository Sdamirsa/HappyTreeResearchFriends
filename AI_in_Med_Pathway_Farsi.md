# ورژن 3.2 مسیر یادگیری کد زدن برای افرادی با بک گراند پزشکی :)
سلام ، اینجا من براتون کلیات مسیری که باید برید رو گذاشتم. دوره های خیلی زیادی هست و هر کدوم رو که دیدید، فرقی نداره، مهم اینه که این چیزایی که نوشته شده رو یادبگیرید و برید مرحله بعدی.
### 1: نصب پایتون و آناکندا و یادگرفتن اینکه ویرچوال اینوایرمنت چیه و جایی که توش کد میزنید یعنی وی اس کد

```mermaid
graph TD
    subgraph Setup_Env
        direction TB
        Anaconda[<a href="https://freelearning.anaconda.cloud/get-started-with-anaconda">Anaconda and Virtual Environment Importance</a>]
        VSCode[<a href="https://www.youtube.com/watch?v=B-s71n0dHUk">VS Code Tour</a>]
        PythonSetup[<a href="https://www.youtube.com/watch?v=qI3P7zMMsgY">Python Environment Setup</a>]

        Anaconda --> VSCode
        VSCode --> PythonSetup
    end
```

### 2: سقوط آزاد در کد زدن
```mermaid
graph TD
    subgraph Code_Path
        direction TB
        DataAnalysis[<a href="https://www.datacamp.com/tracks/data-analyst-with-python">اول دیتا آنالیست</a>]
        LogicCourse[<a href="https://www.youtube.com/playlist?list=PLUl4u3cNGP63WbdFxL8giv4yhgdMGaZNA">کورس منطق کد زدن ام آی تی</a>]
        Projects[بعد یک پروژه آنالیز یا بازی با یک دیتا انجام بدید که تو ذهنتون ماندگار بشه]
        DataCampProjects[میتونید از خود datacamp پروژه هاشو انجام بدید]
        SmallTask[از من یه کار کوچیک بگیرید]
        OwnProject[یا اگر تو خودتون میبینید، یه پروژه انجام بدید که یه پیپیرم معمولی بشه]
        MLPath[<a href="https://www.datacamp.com/tracks/machine-learning-scientist-with-python"> ادامه مسیر کد برای ماشین لرنینگ با دوره دیتاکمپ</a>]

        DataAnalysis --> LogicCourse
        LogicCourse --> Projects
        Projects ---or1[یا]--> DataCampProjects -->MLPath
        Projects ---or2[یا]--> SmallTask-->MLPath
        Projects ---or3[یا]--> OwnProject --> MLPath
        
    end

    MLPath --> MLProject
    MLProject[تموم کردن منطق یادگیری ماشین و انجام پروژه]

```

### 3: منطق یادگیری ماشین


```mermaid
graph TD
    subgraph Pre_ML[پیش نیاز: جبر خطی ]
        Essence[<a href="https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab">چکیده جبر خطی</a>]
        FullCourse[<a href="https://www.youtube.com/watch?v=JnTa9XtvmfI">دوره کامل جبر خطی</a>]
    end

    subgraph ML[یادگیری منطق ماشین]
        LearnLogic[یادگیری منطق پشت ماشین‌لرنینگ و مدل‌ها]
        HealthcareML[<a href="https://www.youtube.com/playlist?list=PLUl4u3cNGP60B0PQXVQyGNdCyCTDU1Q5j">ماشین‌لرنینگ برای بهداشت : کورس ام آی تی</a>]
        StanfordML[<a href="https://youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU&si=uqVtGLVlx0QjYVHW">ریاضیات پشت مدل‌ها: کورس اندرو ان‌جی</a>]
        QuickIntro[معرفی سریع کانسپت‌ها]
        MLasMD1[<a href="https://youtu.be/i2uYaVh9LSc">MLasMD 1 by me</a>]
        MLasMD2[<a href="https://youtu.be/i2uYaVh9LSc">MLasMD 2 by me</a>]
        MakingFriends[<a href="https://youtube.com/playlist?list=PLRKtJ4IpxJpB_2ei8-5eWU31EZ6uSj9_s&si=550kUZ8RAIROjCCW">دوستی با ماشین‌لرنینگ</a>]
        Book[شبا قبل خواب
        Hands on Machine Learning with Python]
    end

        Essence -->|اگر نیاز داشتید | FullCourse

        ML <--> Pre_ML 
        LearnLogic --> HealthcareML
        LearnLogic --> StanfordML
        LearnLogic --> QuickIntro
        QuickIntro --> MLasMD1 --> Book
        QuickIntro --> MLasMD2 --> Book
        QuickIntro --> MakingFriends --> Book
        

        Book-->SelfLearning[تموم کردن مسیر کد و انجام یک پروژه]
```
