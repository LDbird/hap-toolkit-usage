## hap-toolkit新增重新签名的示例

hap-toolkit的0.7.2版本，增加项目重新签名的能力，新增命令行 resign；

可通过命令行 npx hap -v 查看hap-toolkit版本号；

执行 npm run resign，项目根目录下会生成dest目录，在此目录下生成rpk/rpks文件；

quickapp.config.js文件中配置cli属性；执行 npm run resign，相当于执行 npx hap resign --sign sign/release
```
cli: {    
    sign: 'sign/release'
}
```