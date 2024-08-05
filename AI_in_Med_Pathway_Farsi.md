# ورژن 3.2 مسیر یادگیری کد زدن برای افرادی با بک گراند پزشکی :)
سلام ، اینجا من براتون کلیات مسیری که باید برید رو گذاشتم. دوره های خیلی زیادی هست و هر کدوم رو که دیدید، فرقی نداره، مهم اینه که این چیزایی که نوشته شده رو یادبگیرید و برید مرحله بعدی.
### 1: نصب پایتون و آناکندا و یادگرفتن اینکه ویرچوال اینوایرمنت چیه و جایی که توش کد میزنید یعنی وی اس کد
```mermaid
graph BT
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
graph BT
    subgraph Code_Path
        direction TB
        DataAnalysis[<a href="https://www.datacamp.com/tracks/data-analyst-with-python">اول دیتا آنالیست</a>]
        LogicCourse[<a href="https://www.youtube.com/playlist?list=PLUl4u3cNGP63WbdFxL8giv4yhgdMGaZNA">کورس منطق کد زدن ام آی تی</a>]
        Projects[بعد یک پروژه آنالیز یا بازی با یک دیتا انجام بدید که تو ذهنتون ماندگار بشه]
        DataCampProjects[میتونید از خود datacamp پروژه هاشو انجام بدید]
        SmallTask[از من یه کار کوچیک بگیرید]
        OwnProject[یا اگر تو خودتون میبینید، یه پروژه انجام بدید که یه پیپیرم معمولی بشه]
        MLPath[<a href="https://www.datacamp.com/tracks/machine-learning-scientist-with-python"> ادامه مسیر کد برای ماشین لرنینگ با دوره دیتاکمپ</a>]
        MLProject[بعد هم باز یه پروژه ماشین لرنینگ کوچیک انجام بدید]

        DataAnalysis --> LogicCourse
        LogicCourse --> Projects
        Projects ---or1[یا]--> DataCampProjects -->MLPath
        Projects ---or2[یا]--> SmallTask-->MLPath
        Projects ---or3[یا]--> OwnProject --> MLPath
        MLPath --> MLProject
    end
```
