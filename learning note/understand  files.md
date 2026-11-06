## 文件名.ioc
这是cubeMX的图形配置文件，打开就可以进入图形配置页面
## main.c
主程序入口文件，90%的代码写在此处\
代码写在 /* USER CODE BEGIN ... */ 和 /* USER CODE END ... */ 之间\
>>main.h相当于目录，一般不用看 \
>>一般在core目录下\

**主循环 while(1) 里写业务逻辑**

## stm32f1xx_it.c
中断服务函数（Interrupt Handler）集合：SysTick_Handler、EXTI0_IRQHandler、USART1_IRQHandler 等\

需要写**中断处理**时改，回调也要放在 USER CODE 区
