## Quan ly các vai trò và quyền hạn trong hệ thống
cap-contracts/contracts/access/Access.sol 
cap-contracts/contracts/access/AccessControl.sol

## Ủy quyền restaking
# Xử lý ủy uyền tài sản từ các vault đến các nhà cung cấp dịch vụ restaking
cap-contracts/contracts/delegation/Delegation.sol

# Các hợp đồng cụ thể để tương tác với mạng lưới restaking của Symbiotic
# Gửi tài sản đến đó và nhận lại phần thưởng
cap-contracts/contracts/delegation/providers/symbiotic/SymbioticNetwork.sol
cap-contracts/contracts/delegation/providers/symbiotic/SymbioticNetworkMiddleware.sol

## Xử lý fee
# Tổ chức đấu giá để xử lý hoặc phân phối các khoản phí mà giao thức thu được
cap-contracts/contracts/feeAuction/FeeAuction.sol

## Xử lý lendingPool
# Hợp đồng trung tâm của thị trường tiền tệ, xử lý các giao dịch mượn và vay
cap-contracts/contracts/lendingPool/Lender.sol
# Các thư viện chứa logic nghiệp vụ chi tiết cho các hoạt động cho vay
cap-contracts/contracts/lendingPool/libraries/BorrowLogic.sol
cap-contracts/contracts/lendingPool/libraries/LiquidationLogic.sol
cap-contracts/contracts/lendingPool/libraries/ReserveLogic.sol
cap-contracts/contracts/lendingPool/libraries/ValidationLogic.sol
cap-contracts/contracts/lendingPool/libraries/ViewLogic.sol
cap-contracts/contracts/lendingPool/libraries/configuration/AgentConfiguration.sol
cap-contracts/contracts/lendingPool/libraries/math/MathUtils.sol 
cap-contracts/contracts/lendingPool/libraries/math/PercentageMath.sol
cap-contracts/contracts/lendingPool/libraries/math/WadRayMath.sol

# Các contract định nghĩa các loại token đặc biệt như token ghi nợ của người dùng trong hệ thống.
cap-contracts/contracts/lendingPool/tokens/DebtToken.sol
cap-contracts/contracts/lendingPool/tokens/base/MintableERC20.sol
cap-contracts/contracts/lendingPool/tokens/base/ScaledToken.sol

## Cung cấp giá ----------------------------> Đã xong
cap-contracts/contracts/oracle/Oracle.sol
cap-contracts/contracts/oracle/PriceOracle.sol
cap-contracts/contracts/oracle/RateOracle.sol
# Các adapter (bộ chuyển đổi) để lấy dữ liệu từ nhiều nguồn khác nhau
cap-contracts/contracts/oracle/libraries/AaveAdapter.sol
cap-contracts/contracts/oracle/libraries/CapTokenAdapter.sol
cap-contracts/contracts/oracle/libraries/ChainlinkAdapter.sol
cap-contracts/contracts/oracle/libraries/VaultAdapter.sol

## Các contract lưu trữ các giá trị -------------------> Đã xong
cap-contracts/contracts/storage/AccessStorageUtils.sol
cap-contracts/contracts/storage/DebtTokenStorageUtils.sol
cap-contracts/contracts/storage/DelegationStorageUtils.sol
cap-contracts/contracts/storage/FeeAuctionStorageUtils.sol
cap-contracts/contracts/storage/FractionalReserveStorageUtils.sol
cap-contracts/contracts/storage/LenderStorageUtils.sol
cap-contracts/contracts/storage/MintableERC20StorageUtils.sol
cap-contracts/contracts/storage/MinterStorageUtils.sol
cap-contracts/contracts/storage/PriceOracleStorageUtils.sol
cap-contracts/contracts/storage/RateOracleStorageUtils.sol
cap-contracts/contracts/storage/ScaledTokenStorageUtils.sol
cap-contracts/contracts/storage/StakedCapStorageUtils.sol
cap-contracts/contracts/storage/SymbioticNetworkMiddlewareStorageUtils.sol
cap-contracts/contracts/storage/SymbioticNetworkStorageUtils.sol
cap-contracts/contracts/storage/VaultAdapterStorageUtils.sol
cap-contracts/contracts/storage/VaultStorageUtils.sol

## Các contract token
cap-contracts/contracts/token/CapToken.sol
cap-contracts/contracts/token/StakedCap.sol
cap-contracts/contracts/vault/FractionalReserve.sol

## Các contract vault
cap-contracts/contracts/vault/Minter.sol
cap-contracts/contracts/vault/Vault.sol

## Các contract logic
cap-contracts/contracts/vault/libraries/FractionalReserveLogic.sol
cap-contracts/contracts/vault/libraries/MinterLogic.sol
cap-contracts/contracts/vault/libraries/VaultLogic.sol