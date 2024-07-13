- `npx create-nx-workspace my-nest-monorepo --preset=nest`
- `nx add @nx/nest`
- `nx g @nx/nest:app microservice-1 --e2eTestRunner none`
- `nx g @nx/nest:app microservice-2 --e2eTestRunner none`
- `nx g @nx/nest:app microservice-3 --e2eTestRunner none`
- `nx g @nx/nest:lib common --publishable --importPath=@myorg/common --directory libs`
- `nx g @nx/nest:lib common --publishable --importPath=@myorg/influx --directory libs`

- `cd apps/microservice-<1..3>`
- `npm init -y`
- `npm i -S <deps>`

- Add workspaces to root `package.json`
- Removed dependencies from root `package.json`

- `nx build microservice-<1..3>`
