<p align="center">
  <img src="https://raw.githubusercontent.com/xReverseLabs/.github/main/profile/Banner.png" alt="xReverseLabs Logo">
</p>

<h1 align="center">Welcome to xReverseLabs</h1>

<p align="center">
  <b>Innovative OSINT Solutions for Cybersecurity Experts</b><br>
  Empowering penetration testers and security researchers with cutting-edge tools and intelligence for comprehensive domain reconnaissance.
</p>

<p align="center">
  <a href="https://xreverselabs.my.id"><img alt="Website" src="https://img.shields.io/badge/Website-xReverseLabs-blue?style=flat-square"></a>
  <a href="https://github.com/xReverseLabs"><img alt="GitHub followers" src="https://img.shields.io/github/followers/xReverseLabs?style=flat-square"></a>
  <a href="https://linkedin.com/in/bayujsantoso"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Bayu%20Jumhari%20Cahyono-blue?style=flat-square"></a>
  <a href="https://instagram.com/bayujsantoso_"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-%40bayujsantoso__-red?style=flat-square"></a>
</p>

---
## 🌐 xReverseLabs API Documentation

Welcome to the **xReverseLabs API** documentation! 🚀 This API provides various endpoints for managing API keys and performing operations such as reverse IP lookups and subdomain scanning.

## 🔗 Base URL

`https://api.xreverselabs.my.id/`

## 📌 Endpoints

### 1. Reverse IP
- **Endpoint**: `/itsuka` or `/himawari`
- **Method**: `GET`
- **Description**: Retrieves the domains associated with a specific IP address.
- **Query Parameters**:
  - `🔑 apiKey` (string, required) - Your API key.
  - `🌐 ip` (string, required) - The IP address to reverse.
- **Example**:
  - `/itsuka?apiKey=freetrial&ip=101.50.1.10`
- **Response**:
  ```json
  {
    "ip": "101.50.1.10",
    "domains": [
      "7seasmarineproduct.com",
      "batu13.com",
      "cvkam.com"
    ],
    "total": 3
  }
  ```

### 2. Subdomain Scanner
- **Endpoint**: `/subdomain`
- **Method**: `GET`
- **Description**: Scans and retrieves subdomains for a given domain.
- **Query Parameters**:
  - `🔑 apiKey` (string, required) - Your API key.
  - `🌐 url` (string, required) - The domain to scan.
- **Example**:
  - `/subdomain?apiKey=freetrial&url=xreverselabs.my.id`
- **Response**:
  ```json
  {
    "domain": "xreverselabs.my.id",
    "subdomains": [
      "api.xreverselabs.my.id",
      "cloud.xreverselabs.my.id",
      "apiv2.xreverselabs.my.id"
    ],
    "total": 3
  }
  ```

### 3. Domain Grabber By Date
- **Endpoint**: `/domainbydate`
- **Method**: `GET`
- **Description**: Scans and retrieves registered domains by date.
- **Query Parameters**:
  - `🔑 apiKey` (string, required) - Your API key.
  - `📊 date` (string, required) - Date.
  - `🌐 page` (string, required) - Page.
- **Example**:
  - `/domainbydate?apiKey=freetrial&date=2023-01-01&page=2`
- **Response**:
  ```json
  {
    "date": "2023-01-01",
    "domains": [
      "example.site.com",
      "example2.site.com",
      "example3.site.com"
    ],
    "total": 3
  }
  ```

### 4. Reverse IPv6
- **Endpoint**: `/reverse/ipv6`
- **Method**: `GET`
- **Description**: Retrieves the domains associated with a specific IPv6 address.
- **Query Parameters**:
  - `🔑 apiKey` (string, required) - Your API key.
  - `🌐 ip` (string, required) - The IP address to reverse.
- **Example**:
  - `/reverse/ipv6?apiKey=freetrial&ip=100f:xxxxxxx`
- **Response**:
```json
{
  "ip": "100f:xxxxxxx",
  "domains": [
    "12stepsforlivingfree.com",
    "1stclasscloud.com",
    "1takesuccess.com",
    "1to1speechtherapy.com",
    "3tigermartialarts.com"
	],
  "total": 5
}
```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💡 Acknowledgements

- Thanks to the open-source community for their invaluable resources.
- Special thanks to ProjectDiscovery for their excellent tools and inspiration.
- Thanks to xReverseLabs Team
