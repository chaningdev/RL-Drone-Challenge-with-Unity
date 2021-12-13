# 2021 RL Korea Drone Delivery Challenge with Unity
`2021.11.1` ~ `2021.12.07`


**TEAM**: NewBe ([chaningdev](https://github.com/chaningdev), [20170375](https://github.com/20170375))
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    [🎖Unity특별상](https://github.com/reinforcement-learning-kr/2021_RLKR_Drone_Delivery_Challenge_with_Unity/discussions/29#discussion-3729231)

[<img width="1680" alt="main" src="https://user-images.githubusercontent.com/62216628/140608027-bb7cf7d0-ec9e-4a0c-b81a-f89518d1262a.png">](https://github.com/reinforcement-learning-kr/2021_RLKR_Drone_Delivery_Challenge_with_Unity)

    ml-agents: 0.27.0
<hr>



## Examples
<img src="https://user-images.githubusercontent.com/62216628/145405453-79d3c2d8-922a-487a-b419-c7723b2faa63.gif">

+ Reward Parameters
    - Reward = 100
    - Penalty = -100
    - distanceRewardScale = 1

Reward 100값 기준 MAX Reward = 300 + a (distanceRewardScale값에 따름)
    
## Strategy

+ 방향
    <ol>
        <li> Reward 획득을 3번(MAX)을 안정적으로 수행 </li>
        <li> MAX Reward를 달성하는 시간 단축</li> 
    </ol>

+ 안정적 MAX Reward 달성을 위한 방식

    <ol>
    <li> Curiosity Intrinsic Reward 추가</li>
    <li> 5m Steps 마다 변화(Pulse)를 부여</li>
    </ol>


## Models
+ Default + Curiosity Intrinsic Reward [c01]
<img src="https://user-images.githubusercontent.com/84086347/145740730-ebd00286-f1cc-4876-95ca-d91b50ecb8f9.png" width ="500px">
<img src = "https://user-images.githubusercontent.com/84086347/145741971-1f5daf94-d1f5-4b43-95d9-038cd5d5fe92.png" width = "500px")>


+ Training to get high scores [a01_1201]
<img src="https://user-images.githubusercontent.com/62216628/145665627-907305b3-4b37-4e22-8889-1f4005fa80f5.png" width="500px">
<img src="https://user-images.githubusercontent.com/84086347/145742270-c9b2e20c-0f69-4b93-8814-40173923eb0a.png" width = "500px">



+ Overfitting for reducing time [b07_1201_1316]
<img src="https://user-images.githubusercontent.com/62216628/145665695-c9f022ca-1851-45a2-8fc1-d2854d57e0c7.png" width="500px">

+ [Google Drive](https://drive.google.com/drive/folders/1rSW0sPKJGle1PeBhMLt9hs2hPtk8eQdy?usp=sharingd=0)


## Test reports
+ [Google Sheets](https://docs.google.com/spreadsheets/d/1Y6WSbXNk_P0MV6bGyRcPi8gKUHHSR6rwLW71wpur1wM/edit?usp=sharing)


## [Try training](https://github.com/reinforcement-learning-kr/2021_RLKR_Drone_Delivery_Challenge_with_Unity/blob/master/docs/run_with_ml-agents.md#training)


## Reference
+ [2021_RLKR_Drone_Delivery_Challenge_with_Unity](https://github.com/reinforcement-learning-kr/2021_RLKR_Drone_Delivery_Challenge_with_Unity)
+ [ml-agents](https://github.com/Unity-Technologies/ml-agents)
+ [parameter instruction](https://github.com/Unity-Technologies/ml-agents/blob/main/docs/Training-Configuration-File.md)
+ [tensorboard analysis instruction](https://github.com/Unity-Technologies/ml-agents/blob/main/docs/Using-Tensorboard.md)
