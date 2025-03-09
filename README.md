# .openaiao
Open AIAO is an open standard that enables AI agents to interact with websites through structured metadata, similar to how SEO optimizes for search engines.

# Open AIAO - AI Agent Optimization

## The Open Standard for AI Agent Optimization
AIAO (AI Agent Optimization) is a revolutionary open standard that enables AI agents to seamlessly interact with websites and services using structured metadata. Just like SEO helps search engines understand web content, AIAO makes the internet AI-friendly by providing a standardized protocol for AI-driven automation.

## Why AIAO?
AIAO creates an AI-ready internet by making web content machine-readable, reducing automation overhead for businesses and developers. It is an open and extensible standard designed to support multiple industries.

## What is AIAO?
AIAO defines a structured metadata format (JSON-LD) that allows AI agents to:
- Retrieve business information such as hours, services, and contact details.
- Automate tasks like booking appointments and placing orders.
- Interact with industry-specific services, including e-commerce, healthcare, and finance.

## AIAO and Schema.org Integration
AIAO leverages [Schema.org](https://schema.org/) to ensure compatibility with existing structured data standards. By aligning with Schema.org, AIAO metadata can be easily adopted by search engines, AI agents, and automation tools, enhancing interoperability across platforms.

### Example AIAO Metadata with Schema.org (JSON-LD)
```json
{
    "@context": ["https://aiao.org/context", "https://schema.org"],
    "@type": "LocalBusiness",
    "name": "TechGizmo Repair Shop",
    "description": "An AI-friendly tech repair shop",
    "address": {
        "@type": "PostalAddress",
        "streetAddress": "123 Tech Street",
        "addressLocality": "New York",
        "addressRegion": "NY",
        "postalCode": "10001",
        "addressCountry": "US"
    },
    "telephone": "+1-555-123-4567",
    "email": "support@techgizmo.com",
    "url": "https://techgizmo.com",
    "openingHours": "Mo-Fr 09:00-18:00, Sa 10:00-16:00",
    "potentialAction": [
        {
            "@type": "ReserveAction",
            "name": "Schedule Appointment",
            "target": {
                "@type": "EntryPoint",
                "urlTemplate": "https://techgizmo.com/aiao/schedule",
                "actionPlatform": ["http://schema.org/DesktopWebPlatform", "http://schema.org/MobileWebPlatform"],
                "httpMethod": "POST"
            }
        }
    ]
}
```

## How It Works
1. AIAO-optimized websites expose structured metadata at `/aiao/metadata`.
2. AI agents query this metadata to discover available actions.
3. Automation happens as AI agents execute tasks via defined AIAO endpoints.

## Get Started
### Implement AIAO on Your Website
Add an `/aiao/metadata` endpoint with structured JSON-LD data. Refer to the [AIAO API Starter Guide](https://github.com/OpenAIAO/docs) for setup instructions.

### Build an AI Agent that Uses AIAO
Develop an AI assistant that reads AIAO metadata and automates tasks. Refer to the [Python AI Agent Example](https://github.com/OpenAIAO/ai-agent) for guidance.

### Contribute to the Open Standard
AIAO is a community-driven initiative. Join the discussion and contribute to improving the standard on GitHub.

## Join the Movement
Website (coming soon):: [https://openaiao.org](https://openaiao.org)  
GitHub: [https://github.com/OpenAIAO](https://github.com/OpenAIAO)  
X (coming soon): [https://twitter.com/openaiao](https://twitter.com/openaiao)  

## License
AIAO is open-source under the Apache 2.0 License. Contributions are welcome.

---
Open AIAO - Making the web AI-friendly, one website at a time.
