# 实现用户注册功能#

## 开发约定:
- 不能直接访问jsp，只能走#    servlet然后再到jsp
```
    // 遍历 MAP
    Map<String, String[]> map = req.getParameterMap();
    Set<String> keySet = map.keySet();
    Iterator<String> iterator = keySet.iterator();
    while(iterator.hasNext()){
        String str = iterator.next();
        String[] strs = map.get(str);
        for(String str : strs){
            System.out.pringln(str);
        }
    }
```
*tips*
1. alt + /   //　构造午餐函数
1. alt + shift + s // source菜单
1. 选择字符串　＋ctrl+shift+ r　//　快速找到类文件
1. tomcat下的日志信息，记录了当前接口请求的各样信息，也能查到谁请求的，例如ip
1. eclipse -> window -> java -> debug -> Suspend exe....on uncaught exceptions 单选勾去掉 方便断点调试（软件bug）
