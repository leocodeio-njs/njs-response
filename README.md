#### Response Module

```bash
pnpm add @nestjs/config @nestjs/terminus @nestjs/swagger @nestjs/axios prom-client @nestjs/typeorm
```

```typescript
// import helath module
import { ResponseInterceptor } from '@leocodeio-njs/njs-response';

// Add the interceptor to the imports array of your main file
import { ResponseInterceptor } from './response.interceptor';

async function bootstrap() {
  app.useGlobalInterceptors(new ResponseInterceptor());
}
bootstrap();
```
