# Ujnotes
### ujnotes.com

Welcome to Ujnotes

This project houses the software sub system for my blog website: ujnotes.com

## Projects
1. web: [website](https://github.com/ujnotes/web-site)  
main: [web](https://github.com/ujnotes/web)

## Project stcuture

```
Web
│
├── Site
│   └── Project             (ujnotes/web-site)
|       ├── root\framework  (blank-org/cutie - submoduled)
│       ├── interim
│       └── public
│
├── Project                 (ujnotes/web)
│   ├── interim             (ujnotes/web-interim)
│   └── public              (ujnotes/web-public > ujnotes.com)
|
│
└── Tiggu                   (blank-org/tiggu)
│
└── Firebase                (blank-org/firebase)
```

## Steps:  
1. Setup:
    1. Create docker:  
        1. /web  
            This will create :  
                1. web-site  
                2. nginx-proxy

2. Operate:
    1. Update article in CMS  
    2. RUN [NCMS](https://github.com/blank-org/ncms)

3. Deploy:  
    1. Run `render.sh` - [tiggu](https://github.com/blank-org/tiggu)  
    2. push `project\build\public` for CI/CD

