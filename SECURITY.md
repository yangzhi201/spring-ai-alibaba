## Reporting a Vulnerability

Please report any security issue or Higress crash report to [ASRC](https://security.alibaba.com/)(Alibaba Security Response Center) where the issue will be triaged appropriately.

Thank you in advance for helping to keep Spring AI Alibaba secure.
## 报告漏洞

请将任何安全问题或 Higress 崩溃报告提交至 [ASRC](https://security.alibaba.com/)（阿里巴巴安全应急响应中心），相关 issue 将会得到妥善分类与处理。

感谢您提前协助保障 Spring AI Alibaba 的安全。

## 安全最佳实践

1. 及时升级：请始终使用最新版本，以获取最新的安全补丁。  
2. 最小权限：部署时遵循最小权限原则，仅开放必要的端口与访问权限。  
3. 配置审计：定期检查配置文件，确保未暴露敏感信息（如 AccessKey、密码等）。  
4. 依赖扫描：使用 SCA 工具（如 OWASP Dependency-Check）扫描第三方依赖，及时修复已知漏洞。  
5. 监控告警：开启日志与监控，对异常登录、高频请求等行为实时告警。  
6. 密钥管理：推荐使用阿里云 KMS 等托管服务管理密钥，禁止在代码仓库中硬编码密钥。  

如发现文档中安全指引不足，欢迎通过 Issue 或 Pull Request 补充。
