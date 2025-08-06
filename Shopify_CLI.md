# 1. Lệnh cơ bản

## Thông tin & Help:
```bash
shopify version                    # Xem phiên bản CLI
shopify help                       # Xem tất cả lệnh
shopify help [command]             # Xem help cho lệnh cụ thể

shopify upgrade                    # Cập nhật CLI lên version mới
```

## Xác thực:

```bash
shopify auth login                 # Đăng nhập Shopify account
shopify auth logout                # Đăng xuất

shopify auth whoami                # Xem thông tin user hiện tại
```

# 2. Phát triển giao diện

## Phát triển:

```bash
shopify theme dev                  # Chạy development server (localhost)
shopify theme dev --store [store]  # Dev server cho store cụ thể
shopify theme dev --theme-id [id]  # Dev với theme ID cụ thể

shopify theme dev --port [port]    # Chỉ định port (mặc định 9292)
shopify theme dev --host [host]    # Chỉ định host (mặc định 127.0.0.1)
shopify theme dev --poll           # Dùng polling thay vì file watching


shopify theme pull                 # Pull theme hiện tại
shopify theme pull --theme-id [id] # Pull theme ID cụ thể
shopify theme pull --live          # Pull live theme

shopify theme pull --development   # Pull development theme
shopify theme pull --path [path]   # Pull vào thư mục cụ thể
shopify theme pull --nodelete      # Không xóa files local
```

## Triển khai:

```bash
shopify theme push                 # Push theme hiện tại
shopify theme push --allow-live    # Cho phép push lên live theme
shopify theme push --unpublished   # Tạo theme unpublished

shopify theme push --theme-id [id] # Push lên theme ID cụ thể
shopify theme push --path [path]   # Push từ thư mục cụ thể
shopify theme push --live          # Push lên live theme (NGUY HIỂM!)
shopify theme push --json          # Output dạng JSON
```

## Các công cụ khác:

```bash
shopify theme check                # Validate theme code

shopify theme check --category [c] # Check theo category cụ thể
shopify theme check --severity [s] # Check theo mức độ nghiêm trọng
shopify theme check --list         # Liệt kê tất cả rules


shopify theme info                 # Xem thông tin theme hiện tại
shopify theme list                 # Liệt kê tất cả themes

shopify theme list --name [name]   # Filter theo tên
shopify theme list --role [role]   # Filter theo role
shopify theme list --json          # Output dạng JSON


shopify theme publish              # Publish theme hiện tại
shopify theme publish --theme-id [id] # Publish theme cụ thể

shopify theme publish --force      # Publish không cần confirm


shopify theme share                # Tạo preview link
shopify theme share --theme-id [id] # Share theme cụ thể


shopify theme rename [new-name]    # Đổi tên theme hiện tại
shopify theme rename [name] --theme-id [id] # Đổi tên theme cụ thể


shopify theme delete               # Xóa theme hiện tại
shopify theme delete --theme-id [id] # Xóa theme ID cụ thể
shopify theme delete --development # Xóa development theme

shopify theme delete --force       # Xóa không cần confirm


shopify system                     # Xem thông tin hệ thống
shopify system doctor              # Kiểm tra system health
shopify system environment         # Xem environment variables


shopify --verbose [command]        # Chạy với verbose output
shopify --debug [command]          # Chạy với debug mode
```

# 3. Function Extensions

## Biên dịch và chạy:

```bash
shopify app function build         # Build function thành WebAssembly
shopify app function run           # Chạy thử function tại local

shopify app function replay        # Replay function với payload để debug
```

## Công cụ hỗ trợ:

```bash
shopify app function schema        # Sinh file schema.graphql mới
shopify app function typegen       # Tạo type cho GraphQL truy vấn
```

# 4. Lệnh tiện ích khác

## Cấu hình:

```bash
shopify config                     # Xem config hiện tại

shopify config get [key]           # Lấy giá trị key
shopify config set [key] [value]   # Set giá trị cho key
shopify config unset [key]         # Xóa key
```

## Tìm kiếm:

```bash
shopify search                     # Tìm kiếm tài liệu từ CLI
```
