# luyou
路由基本搭建

 
      import { createBottomTabNavigator } from "react-navigation";

      const DBRoute = createBottomTabNavigator(
        {
          One: {
            screen: TopRoute,
            navigationOptions: {
              title: ""
            }
          },
          Two: {
            screen: Two,
            navigationOptions: {
              title: ""
            }
          }
        },
        {
          //设置文本选中前后效果颜色
          tabBarOptions: {
            activeTintColor: "white", //激活样式
            inactiveTintColor: "gray" //未激活样式
          },
          tabBarPosition: "top", //设置显示位置
          swipeEnabled: true, //是否可以滑动
          animationEnabled: true //滑动效果
        }
      );

      export default DBRoute;
