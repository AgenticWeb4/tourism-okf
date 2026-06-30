# tourism-okf

Open Knowledge Format (OKF) bundles for Tourism agents — git-native, vendor-neutral.

## Layout

```text
tour-guide/                 # Canonical bundle (agent consumption root)
└── destinations/
    └── xian/               # 西安（Phase 1）
```

## Authoring

See [CONTRIBUTING.md](./CONTRIBUTING.md). Validate before merge:

```bash
okf-lint lint --bundle tour-guide
```

## License

Content © contributors. OKF structure follows [okf.md](https://okf.md/) v0.1.
