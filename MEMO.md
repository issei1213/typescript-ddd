## Dockerの立ち上げ方
```bash
docker compose up -d
npx prisma migrate dev --name init
```

## Express サーバー起動
```bash
npx ts-node src/Presentation/Express/index.ts
```

## 書籍登録APIをCurl
```bash
curl -X POST -H "Content-Type: application/json" -d '{"isbn":"9784167158057","title":"吾輩は猫である","priceAmount":770}' http://localhost:3000/book
```

## Prisma GUI
```bash
npx prisma studio
```