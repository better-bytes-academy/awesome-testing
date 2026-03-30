# Performance Testing Tools

> Tổng hợp các công cụ kiểm thử hiệu năng.

---

## 📌 Mục lục

- [Load Testing Tools](#load-testing-tools)
- [Browser Performance Tools](#browser-performance-tools)
- [APM & Monitoring](#apm--monitoring)
- [Benchmarking Tools](#benchmarking-tools)

---

## Load Testing Tools

| Công cụ | Ngôn ngữ | Giá | Mô tả | Link |
|---------|---------|-----|-------|------|
| **JMeter** | Java | Free | Công cụ load test phổ biến nhất, GUI-based | [jmeter.apache.org](https://jmeter.apache.org/) |
| **k6** | JavaScript | Free | Modern load testing tool by Grafana | [k6.io](https://k6.io/) |
| **Gatling** | Scala/Java | Free/Paid | Performance testing framework, DSL-based | [gatling.io](https://gatling.io/) |
| **Locust** | Python | Free | Distributed load testing, code-based | [locust.io](https://locust.io/) |
| **Artillery** | JavaScript | Free/Paid | Cloud-native performance testing | [artillery.io](https://artillery.io/) |
| **Vegeta** | Go | Free | HTTP load testing CLI tool | [github.com/tsenart/vegeta](https://github.com/tsenart/vegeta) |
| **wrk** | C | Free | HTTP benchmarking tool | [github.com/wg/wrk](https://github.com/wg/wrk) |
| **BlazeMeter** | - | Paid | Cloud-based, tương thích JMeter | [blazemeter.com](https://www.blazemeter.com/) |
| **LoadRunner** | - | Paid | Enterprise performance testing | [microfocus.com](https://www.microfocus.com/) |

---

## Browser Performance Tools

| Công cụ | Mô tả | Link |
|---------|-------|------|
| **Lighthouse** | Audit performance, SEO, accessibility (built-in Chrome) | [developer.chrome.com](https://developer.chrome.com/docs/lighthouse/) |
| **WebPageTest** | Detailed web performance analysis | [webpagetest.org](https://www.webpagetest.org/) |
| **PageSpeed Insights** | Google's page speed analyzer | [pagespeed.web.dev](https://pagespeed.web.dev/) |
| **GTmetrix** | Performance reports & monitoring | [gtmetrix.com](https://gtmetrix.com/) |
| **Chrome DevTools** | Network, Performance, Memory profiling | Built-in Chrome |

---

## APM & Monitoring

| Công cụ | Giá | Mô tả | Link |
|---------|-----|-------|------|
| **Grafana** | Free/Paid | Dashboards & observability | [grafana.com](https://grafana.com/) |
| **Prometheus** | Free | Monitoring & alerting toolkit | [prometheus.io](https://prometheus.io/) |
| **Datadog** | Paid | Full-stack monitoring platform | [datadoghq.com](https://www.datadoghq.com/) |
| **New Relic** | Free/Paid | Application performance monitoring | [newrelic.com](https://newrelic.com/) |
| **Dynatrace** | Paid | AI-powered observability | [dynatrace.com](https://www.dynatrace.com/) |

---

## Benchmarking Tools

| Công cụ | Mô tả | Link |
|---------|-------|------|
| **ApacheBench (ab)** | CLI HTTP benchmarking | [httpd.apache.org](https://httpd.apache.org/docs/2.4/programs/ab.html) |
| **hey** | HTTP load generator | [github.com/rakyll/hey](https://github.com/rakyll/hey) |
| **siege** | HTTP regression testing & benchmarking | [github.com/JoeDog/siege](https://github.com/JoeDog/siege) |
| **bombardier** | Fast HTTP benchmarking tool (Go) | [github.com/codesenberg/bombardier](https://github.com/codesenberg/bombardier) |

---

## So sánh nhanh các Load Testing Tools

| Tiêu chí | JMeter | k6 | Gatling | Locust |
|---------|--------|----|---------| -------|
| **Ngôn ngữ script** | GUI/XML | JavaScript | Scala/Java | Python |
| **GUI** | ✅ | ❌ | ❌ | Web UI |
| **CI/CD** | ✅ | ✅ | ✅ | ✅ |
| **Protocol** | HTTP, FTP, JDBC, ... | HTTP, WebSocket, gRPC | HTTP, WebSocket | HTTP |
| **Distributed** | ✅ | ✅ (k6 Cloud) | ✅ | ✅ |
| **Learning curve** | Medium | Low | Medium | Low |
| **Report** | Tùy chỉnh | Built-in | HTML report | Web UI |

---

## 📚 Tham khảo

- [Awesome JMeter](https://github.com/aliesbelik/awesome-jmeter)
- [k6 Documentation](https://k6.io/docs/)
- [Performance Testing Guide - Guru99](https://www.guru99.com/performance-testing.html)
